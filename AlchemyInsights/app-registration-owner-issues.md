---
title: 应用注册所有者问题
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
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123064"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="60f47-102">应用注册所有者问题</span><span class="sxs-lookup"><span data-stu-id="60f47-102">App Registration Owner issues</span></span>

<span data-ttu-id="60f47-103">以下是将主体添加为应用注册所有者的可用方法：</span><span class="sxs-lookup"><span data-stu-id="60f47-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="60f47-104">使用 Azure AD PowerShell 模块 -</span><span class="sxs-lookup"><span data-stu-id="60f47-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="60f47-105">参考 [：Add-AzureADApplicationOwner (AzureAD) ](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="60f47-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="60f47-106">使用 Azure CLI - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="60f47-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="60f47-107">参考 [：az 广告应用所有者](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="60f47-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="60f47-108">使用 MS Graph -</span><span class="sxs-lookup"><span data-stu-id="60f47-108">Using MS Graph -</span></span>

    <span data-ttu-id="60f47-109">参考： [添加所有者 - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="60f47-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="60f47-110">使用 Azure AD 门户 - 导航 [到](https://portal.azure.com/) portal.azure.com> Azure Active directory >应用注册>选择应用程序>所有者>添加所有者"</span><span class="sxs-lookup"><span data-stu-id="60f47-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="60f47-111">**即使你是该应用程序的所有者，也无法在"应用注册"边栏选项卡上查看应用程序？**</span><span class="sxs-lookup"><span data-stu-id="60f47-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="60f47-112">应用的所有者不是管理角色。</span><span class="sxs-lookup"><span data-stu-id="60f47-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="60f47-113">如果启用 ["限制对 Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) 管理门户的访问"设置，则只有管理员才能在应用注册门户上查看应用程序。</span><span class="sxs-lookup"><span data-stu-id="60f47-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="60f47-114">若要使所有者能够查看应用程序，请禁用此设置 (将其设置为 NO) 或仅为特定应用程序向所有者分配管理员角色。</span><span class="sxs-lookup"><span data-stu-id="60f47-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="60f47-115">但是，为此，你需要 Azure AD Premium P2 许可证并启用 [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)。</span><span class="sxs-lookup"><span data-stu-id="60f47-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
