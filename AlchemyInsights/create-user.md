---
title: 创建用户
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718172"
---
# <a name="create-user"></a><span data-ttu-id="5bff1-102">创建用户</span><span class="sxs-lookup"><span data-stu-id="5bff1-102">Create user</span></span>

<span data-ttu-id="5bff1-103">**公告：**</span><span class="sxs-lookup"><span data-stu-id="5bff1-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="5bff1-104">[自 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) 年 1 月 4 日起，Google 弃用 WebView 登录支持。</span><span class="sxs-lookup"><span data-stu-id="5bff1-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="5bff1-105">按照 Google 有关测试兼容性的指导测试 [你的应用是否可能](https://go.microsoft.com/fwlink/?linkid=2157323) 受到影响。</span><span class="sxs-lookup"><span data-stu-id="5bff1-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="5bff1-106">请确保在使用消费者 Google 帐户登录用户时使用系统 Webview 或系统浏览器。</span><span class="sxs-lookup"><span data-stu-id="5bff1-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="5bff1-107">有关详细信息，请参阅[仅使用 Chrome 浏览器登陆应用的问题](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)。</span><span class="sxs-lookup"><span data-stu-id="5bff1-107">For more information, see [Issues signing in to application(s) using Chrome browser only](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="5bff1-108">**我无法在我的 Azure AD 目录中创建新用户**</span><span class="sxs-lookup"><span data-stu-id="5bff1-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="5bff1-109">确保你具有创建新的标准用户的权限。</span><span class="sxs-lookup"><span data-stu-id="5bff1-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="5bff1-110">只有 Azure Active Directory (AD) 全局管理员或用户管理员角色才能创建新的标准用户。</span><span class="sxs-lookup"><span data-stu-id="5bff1-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="5bff1-111">如果你不属于上述角色，需请求管理员将你添加到某个上述角色，或让他们为你创建新的用户账户。</span><span class="sxs-lookup"><span data-stu-id="5bff1-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="5bff1-112">确保域中的用户名在你的 Azure AD 中完成过验证。</span><span class="sxs-lookup"><span data-stu-id="5bff1-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="5bff1-113">如果你在 Azure AD 中没有任何验证过的自定义域名，你可以使用以 \*.onmicrosoft.com 结尾的 Azure AD 初始域名。</span><span class="sxs-lookup"><span data-stu-id="5bff1-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="5bff1-114">确保用户名所在域不是从你的本地 AD 上与 Azure AD 联合的域。</span><span class="sxs-lookup"><span data-stu-id="5bff1-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="5bff1-115">无法使用从本地联合的域名将用户添加到云。</span><span class="sxs-lookup"><span data-stu-id="5bff1-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="5bff1-116">确保没有其他用户或联系人已经使用了你想要分配给新用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="5bff1-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="5bff1-117">用户名必须是 Azure AD 中唯一的。</span><span class="sxs-lookup"><span data-stu-id="5bff1-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="5bff1-118">参阅你的 Azure AD 的 [Azure AD 角色和管理员](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)。</span><span class="sxs-lookup"><span data-stu-id="5bff1-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="5bff1-119">参阅你的 Azure AD 的[域名](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)。</span><span class="sxs-lookup"><span data-stu-id="5bff1-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="5bff1-120">检查 [审核日志](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) 来查看关于最近创建的或删除的用户的详细信息，比如谁执行的操作以及何时执行的。</span><span class="sxs-lookup"><span data-stu-id="5bff1-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="5bff1-121">有关添加新用户的信息，请参阅使用 Azure 门户在 [Azure AD](/azure/active-directory/active-directory-users-create-azure-portal)中创建新用户。</span><span class="sxs-lookup"><span data-stu-id="5bff1-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="5bff1-122">[Azure AD 管理角色](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)：Azure Active Directory 中的管理员角色权限</span><span class="sxs-lookup"><span data-stu-id="5bff1-122">[Azure AD administrative roles](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="5bff1-123">您还可以使用 [Azure AD PowerShell 创建新用户](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)。</span><span class="sxs-lookup"><span data-stu-id="5bff1-123">You can also [use Azure AD PowerShell to create a new user](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
