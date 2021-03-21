---
title: 用户管理问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897565"
---
# <a name="user-management-issues"></a><span data-ttu-id="fd399-102">用户管理问题</span><span class="sxs-lookup"><span data-stu-id="fd399-102">User management issues</span></span>

<span data-ttu-id="fd399-103">**如果禁用属性"需要用户分配"（将此属性设置为 No），则当前已分配至应用程序的用户会发生什么情况？**</span><span class="sxs-lookup"><span data-stu-id="fd399-103">**What happens to current assigned users to the application if I disable the property ‘User assignment required’ (set this property to No)?**</span></span>

<span data-ttu-id="fd399-104">禁用 **需要用户分配** 不会影响当前已分配的用户。</span><span class="sxs-lookup"><span data-stu-id="fd399-104">Disabling **User assignment required** does NOT affect the currently assigned users.</span></span> <span data-ttu-id="fd399-105">禁用此属性将仅允许所有用户访问该应用程序。</span><span class="sxs-lookup"><span data-stu-id="fd399-105">Disabling this property will only allow all users to access the application.</span></span> <span data-ttu-id="fd399-106">列出的所有用户和应用程序中分配给组的用户仍然有效。</span><span class="sxs-lookup"><span data-stu-id="fd399-106">All the listed users and those users assigned to groups in the application will still be valid.</span></span>

- <span data-ttu-id="fd399-107">若要将应用限制到特定的一组用户，请参阅 [将Azure AD 应用限制为一组用户 - Microsoft 标识平台|Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.)。</span><span class="sxs-lookup"><span data-stu-id="fd399-107">To restrict your app to specific set of users, see - [Restrict Azure AD app to a set of users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span></span>
- <span data-ttu-id="fd399-108">若要从 Azure 门户内使用 PowerShell 将用户和组分配给 Azure Active Directory （Azure AD） 中的企业应用程序，请参阅 [在 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)中管理应用的用户分配。</span><span class="sxs-lookup"><span data-stu-id="fd399-108">To assign users and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span>
- <span data-ttu-id="fd399-109">若要代理应用程序创建和管理权限，请参阅 [代理应用程序管理管理员权限 - Azure AD |Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles)。</span><span class="sxs-lookup"><span data-stu-id="fd399-109">To delegate Application creation and management permissions, see [Delegate application management administrator permissions - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span></span>
- <span data-ttu-id="fd399-110">**向用户隐藏特定企业应用程序** - 按照以下步骤操作，从 **我的应用** 面板中隐藏所有 Microsoft 365 应用程序。</span><span class="sxs-lookup"><span data-stu-id="fd399-110">**Hide specific enterprise apps from users** - Use the following steps to hide all Microsoft 365 apps from the **MyApps** panel.</span></span> <span data-ttu-id="fd399-111">这些应用仍在 Office 365 门户中可见。</span><span class="sxs-lookup"><span data-stu-id="fd399-111">The apps will still be visible in the Office 365 portal.</span></span>

 1. <span data-ttu-id="fd399-112">以目录的全局管理员登身份登录到 Azure 门户。</span><span class="sxs-lookup"><span data-stu-id="fd399-112">Sign-in to the Azure portal as a global administrator for your directory.</span></span> 
 2. <span data-ttu-id="fd399-113">选择 **Azure Active Directory**。</span><span class="sxs-lookup"><span data-stu-id="fd399-113">Select **Azure Active Directory**.</span></span> 
 3. <span data-ttu-id="fd399-114">选择 **用户**。</span><span class="sxs-lookup"><span data-stu-id="fd399-114">Select **Users**.</span></span> 
 4. <span data-ttu-id="fd399-115">选择 **用户设置**。</span><span class="sxs-lookup"><span data-stu-id="fd399-115">Select **User settings**.</span></span> 
 5. <span data-ttu-id="fd399-116">在 **企业应用程序** 中，点击 **"管理最终用户启动和查看其应用程序**。</span><span class="sxs-lookup"><span data-stu-id="fd399-116">Under **Enterprise applications**, click **Manage how end users launch and view their applications**.</span></span> 
 6. <span data-ttu-id="fd399-117">对于 **用户只能在 Office 365 门户中看到 Office 365 应用程序**，请单击" **是**。</span><span class="sxs-lookup"><span data-stu-id="fd399-117">For **Users can only see Office 365 apps in the Office 365 portal**, click **Yes**.</span></span> 
 7. <span data-ttu-id="fd399-118">单击 **保存**。</span><span class="sxs-lookup"><span data-stu-id="fd399-118">Click **Save**.</span></span> 
 8. <span data-ttu-id="fd399-119">有关详细信息，请参阅 [Azure AD 设备中的用户体验中隐藏企业应用程序|Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span><span class="sxs-lookup"><span data-stu-id="fd399-119">For more details, see [Hide an Enterprise application from user's experience in Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span></span>

- <span data-ttu-id="fd399-120">如果向许多组织提供软件即服务 （SaaS） 应用程序，可以将应用程序配置为接受来自任何 Azure Active Directory （Azure AD） 租户的登录。</span><span class="sxs-lookup"><span data-stu-id="fd399-120">If you offer a Software as a Service (SaaS) app to many organizations, you can configure your app to accept sign-ins from any Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="fd399-121">此配置称为"使应用程序成为多租户"。</span><span class="sxs-lookup"><span data-stu-id="fd399-121">This configuration is called "making your application multi-tenant".</span></span> <span data-ttu-id="fd399-122">任何 Azure AD 租户中的用户在同意通过你的应用程序用其账号后，将能够登录到你的应用程序。</span><span class="sxs-lookup"><span data-stu-id="fd399-122">Users in any Azure AD tenant will be able to sign-in to your app after consenting to use their account with your app.</span></span> <span data-ttu-id="fd399-123">有关详细信息，请参阅 [构建登录 Azure AD 用户的应用程序 - Microsoft 标识平台|Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant)。</span><span class="sxs-lookup"><span data-stu-id="fd399-123">For more information, see [Build apps that sign in Azure AD users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span></span>

- <span data-ttu-id="fd399-124">**最终用户分配到应用程序后如何访问该应用程序？**</span><span class="sxs-lookup"><span data-stu-id="fd399-124">**How can an end user access the application once he/she is assigned to the application?**</span></span>

<span data-ttu-id="fd399-125">企业应用程序模版中的每一个应用程序都有一个链接，供最终用户访问。</span><span class="sxs-lookup"><span data-stu-id="fd399-125">Each app in Enterprise application blade has a link for end users to access.</span></span> <span data-ttu-id="fd399-126">用户还可通过 **我的应用** 门户轻松访问该应用。</span><span class="sxs-lookup"><span data-stu-id="fd399-126">Users can also access the app through **Myapps** portal in an easy way.</span></span>

- <span data-ttu-id="fd399-127">**希望了解用户正在使用哪些应用程序和应用程序类型？**</span><span class="sxs-lookup"><span data-stu-id="fd399-127">**Want to know which applications and type of applications are being used by users?**</span></span>

<span data-ttu-id="fd399-128">可以从 **portal.azure.com >Azure Active Directory>Signins> 下载** 中，下载过去 30 天的登录报告。</span><span class="sxs-lookup"><span data-stu-id="fd399-128">You can download sign-in reports for the last 30 days from **portal.azure.com > Azure Active directory> Signins> download reports**.</span></span>

- <span data-ttu-id="fd399-129">了解如何 [许可授予租户范围的管理员](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) 并 [许可配置最终用户对应用程序](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)。</span><span class="sxs-lookup"><span data-stu-id="fd399-129">Learn how to [Grant tenant wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) and [Configure how end users consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span></span>

- <span data-ttu-id="fd399-130">了解 [许可的工作原理](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 以及 [管理对应用程序的许可](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)。</span><span class="sxs-lookup"><span data-stu-id="fd399-130">Understand [how consent works](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) and [Manage consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span></span>


