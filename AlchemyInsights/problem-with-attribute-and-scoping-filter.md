---
title: 属性和范围筛选器问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430725"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="c354d-102">属性和范围筛选器问题</span><span class="sxs-lookup"><span data-stu-id="c354d-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="c354d-103">**存在 UPN 值冲突的问题**</span><span class="sxs-lookup"><span data-stu-id="c354d-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="c354d-104">“Workday 到 AD 用户设置 Workday 到 AD 用户设置” 显示错误信息 **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**。</span><span class="sxs-lookup"><span data-stu-id="c354d-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="c354d-105">操作失败，因为用于添加/修改的 UPN 值不是全林中唯一的。</span><span class="sxs-lookup"><span data-stu-id="c354d-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="c354d-106">错误详细信息: **CONSTRAINT_ATT_TYPE - userPrincipalName**。</span><span class="sxs-lookup"><span data-stu-id="c354d-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="c354d-107">Workday连接器在创建AD用户账户时试图设置的 **userPrincipalName** 值已经存在于目标 AD 域中。</span><span class="sxs-lookup"><span data-stu-id="c354d-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="c354d-108">这意味着：(1) 用户已经存在，且该用户的匹配 ID 检查失败，或者 (2) UPN生成规则生成了一个冲突值。</span><span class="sxs-lookup"><span data-stu-id="c354d-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="c354d-109">以下是建议的解决步骤：</span><span class="sxs-lookup"><span data-stu-id="c354d-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="c354d-110">如果用户已经存在，并且匹配 ID 检查未能将 Workday 账户链接到 Active Directory 账户，则检查 Workday 和 AD 中的匹配 ID 属性（通常是 **employeeID**）是否完全匹配。</span><span class="sxs-lookup"><span data-stu-id="c354d-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="c354d-111">如果他们没有匹配，则是数据问题，需要解决。</span><span class="sxs-lookup"><span data-stu-id="c354d-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="c354d-112">例如，如果 Workday 中的 EmployeeID 是 001052，而 AD 中的 EmployeeID 是 1052，那么供应引擎将无法链接这两个账户，并将尝试创建一个已经存在的用户。</span><span class="sxs-lookup"><span data-stu-id="c354d-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="c354d-113">本案例的解决方法是改变 AD 中的 **EmployeeID** 值，使其包含前导零成为 001052。</span><span class="sxs-lookup"><span data-stu-id="c354d-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="c354d-114">如果生成 UPN 的表达式没有生成唯一值，可以考虑使用 “去重复函数” **SelectUniqueValue** 来每次生成唯一值。</span><span class="sxs-lookup"><span data-stu-id="c354d-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="c354d-115">**Workday 到 AD 用户设置没有为 AD 用户账户设管理器属性值**</span><span class="sxs-lookup"><span data-stu-id="c354d-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="c354d-116">“Workday 到 AD 用户设置”作业没有为 AD 用户账户设置 **manager** 属性值。</span><span class="sxs-lookup"><span data-stu-id="c354d-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="c354d-117">出现此行为时，有两种可能的情形：</span><span class="sxs-lookup"><span data-stu-id="c354d-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="c354d-118">Workday 中的管理器无法解析到对应的 AD 用户账户，因为该管理器不在范围内。</span><span class="sxs-lookup"><span data-stu-id="c354d-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="c354d-119">在有 **多个 AD 域** 的情形下，Workday 中的管理器与用户不在同一个域中。</span><span class="sxs-lookup"><span data-stu-id="c354d-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="c354d-120">尝试使用以下步骤来解决问题：</span><span class="sxs-lookup"><span data-stu-id="c354d-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="c354d-121">如果已经定义作用域筛选器，请首先检查管理器是否在作用域中，且它是否满足作用域子句。</span><span class="sxs-lookup"><span data-stu-id="c354d-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="c354d-122">如果管理器不满足范围筛选器，请更改筛选器，使管理器也位于供应操作的范围内。</span><span class="sxs-lookup"><span data-stu-id="c354d-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="c354d-123">如果你有多个 AD 域，则连接器具有一个已知的无用限制来解决跨域管理器的引用。</span><span class="sxs-lookup"><span data-stu-id="c354d-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="c354d-124">有关配置 workday 以实现自动设置的更多细节，请参阅 [教程：为自动用户设置配置 Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)。</span><span class="sxs-lookup"><span data-stu-id="c354d-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













