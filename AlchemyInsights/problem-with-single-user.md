---
title: 单个用户的问题
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428569"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="c633f-102">单个用户的问题</span><span class="sxs-lookup"><span data-stu-id="c633f-102">Problem with single user</span></span>

- <span data-ttu-id="c633f-103">用户可能尚未设置，因为服务尚未有机会评估用户。</span><span class="sxs-lookup"><span data-stu-id="c633f-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="c633f-104">查看预配需要的时间以及设置配置页面上的进度栏的指南。</span><span class="sxs-lookup"><span data-stu-id="c633f-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="c633f-105">如果其他详细信息部分中指定的稳定状态是在用户创建/更新/删除日期之前，这意味着我们尚未评估用户。</span><span class="sxs-lookup"><span data-stu-id="c633f-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="c633f-106">在此方案中，最好等待预配服务完成。</span><span class="sxs-lookup"><span data-stu-id="c633f-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="c633f-107">请注意，我们的服务仅知道源系统中用户对云 HR (的更改) 。</span><span class="sxs-lookup"><span data-stu-id="c633f-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="c633f-108">对于 Azure AD，源系统中必须存在有效的更改，以检测更改并流入 Active Directory。</span><span class="sxs-lookup"><span data-stu-id="c633f-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="c633f-109">预配服务评估了用户，并确定了不应进行预配：</span><span class="sxs-lookup"><span data-stu-id="c633f-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="c633f-110">如果已设置基于属性的作用域筛选器，请确保用户满足您指定的条件。</span><span class="sxs-lookup"><span data-stu-id="c633f-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="c633f-111">如果用户已存在于目标系统中，并且源和目标匹配中用户的状态，我们不会执行任何其他操作。</span><span class="sxs-lookup"><span data-stu-id="c633f-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="c633f-112">预配服务尝试设置用户，但失败。</span><span class="sxs-lookup"><span data-stu-id="c633f-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="c633f-113">对于这些方案，请查看预配日志的"疑难解答和建议"选项卡：</span><span class="sxs-lookup"><span data-stu-id="c633f-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="c633f-114">本地 Active Directory 或 Azure AD 中可能缺少用户所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c633f-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="c633f-115">例如，userPrincipalName 或 sAMAccountName 生成规则未生成正确的值。</span><span class="sxs-lookup"><span data-stu-id="c633f-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="c633f-116">匹配属性 (通常是 employeeId) 无法解析为本地 Active Directory 或 Azure AD 中的唯一用户。</span><span class="sxs-lookup"><span data-stu-id="c633f-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="c633f-117">例如，AD 中具有相同 employeeId 的两个用户，服务返回错误代码，指示同一源条目的重复目标条目。</span><span class="sxs-lookup"><span data-stu-id="c633f-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="c633f-118">若要查看单个用户和组的日志，请参阅查看特定用户的问题的预配 [日志](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)。</span><span class="sxs-lookup"><span data-stu-id="c633f-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
