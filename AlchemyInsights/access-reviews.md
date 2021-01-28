---
title: 访问审查
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7767"
ms.openlocfilehash: b2ba50c4f8e667f81b638ba480fa846e149c3d43
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013919"
---
# <a name="access-reviews"></a><span data-ttu-id="b935b-102">访问审查</span><span class="sxs-lookup"><span data-stu-id="b935b-102">Access reviews</span></span>

1. <span data-ttu-id="b935b-103">**启用访问评审**：可以在创建新的访问包或编辑现有访问包时启用评价。</span><span class="sxs-lookup"><span data-stu-id="b935b-103">**Enable Access Reviews**: You can enable reviews when you create a new access package or edit an existing access package.</span></span> <span data-ttu-id="b935b-104">[在 Azure AD 权利](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) 管理中创建访问包的访问评审，介绍如何启用访问包的访问评审。</span><span class="sxs-lookup"><span data-stu-id="b935b-104">[Create an access review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) describes how to enable access reviews of access packages.</span></span>

1. <span data-ttu-id="b935b-105">**Review Access**： Azure AD entitlement management simplifies how enterprises manage access to groups， applications， and SharePoint sites.</span><span class="sxs-lookup"><span data-stu-id="b935b-105">**Review Access**: Azure AD entitlement management simplifies how enterprises manage access to groups, applications, and SharePoint sites.</span></span> <span data-ttu-id="b935b-106">[在 Azure AD](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) 权利管理中查看访问包的访问描述如何对分配了访问包的其他用户执行访问评审，这些用户访问是指定的审阅者。</span><span class="sxs-lookup"><span data-stu-id="b935b-106">[Review access of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) describes how to perform access reviews for other users that are assigned to an access package as a designated reviewer.</span></span>

1. <span data-ttu-id="b935b-107">**自行查看** 访问：在 [Azure AD](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) 权利管理中自审阅访问包描述用户如何自行查看其分配的访问权限 (包) 。</span><span class="sxs-lookup"><span data-stu-id="b935b-107">**Review Access for Yourself**: [Self-review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) describes how a user does a self-review of their assigned access package(s).</span></span>

1. <span data-ttu-id="b935b-108">在大多数情况下，最终用户将在访问面板中查找等待其 **回复的审阅**。</span><span class="sxs-lookup"><span data-stu-id="b935b-108">In most cases, end users will find a review pending their response in the **Access Panel**.</span></span> <span data-ttu-id="b935b-109">这仅适用于组和应用程序审阅，不适用于角色。</span><span class="sxs-lookup"><span data-stu-id="b935b-109">This is only applicable to reviews of Groups and Applications, not Roles.</span></span> <span data-ttu-id="b935b-110">对于角色的所有访问评审，最终用户必须导航到 PIM (Azure AD Privileged Identity Management) 完成审阅。</span><span class="sxs-lookup"><span data-stu-id="b935b-110">For all Access Reviews of roles, end users must navigate to Azure AD Privileged Identity Management (PIM) to complete their review.</span></span>

    1. <span data-ttu-id="b935b-111">登录到 Azure 门户。</span><span class="sxs-lookup"><span data-stu-id="b935b-111">Logon to the Azure portal.</span></span>
    2. <span data-ttu-id="b935b-112">导航到 Azure AD PIM。</span><span class="sxs-lookup"><span data-stu-id="b935b-112">Navigate to Azure AD PIM.</span></span>
    3. <span data-ttu-id="b935b-113">在左侧导航窗格中，选择 **"任务**  >  **审阅访问权限"。**</span><span class="sxs-lookup"><span data-stu-id="b935b-113">In the left navigation pane, select **Tasks** > **Review access**.</span></span>
    
<span data-ttu-id="b935b-114">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="b935b-114">For more information, see:</span></span>

- [<span data-ttu-id="b935b-115">在 PIM 中执行对 Azure AD 目录角色的访问评审 </span><span class="sxs-lookup"><span data-stu-id="b935b-115">Perform an access review of my Azure AD directory roles in PIM </span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-perform-security-review/)
- [<span data-ttu-id="b935b-116">在 PIM 中执行 Azure 资源角色的访问评审</span><span class="sxs-lookup"><span data-stu-id="b935b-116">Perform an access review of my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-perform-access-review/)