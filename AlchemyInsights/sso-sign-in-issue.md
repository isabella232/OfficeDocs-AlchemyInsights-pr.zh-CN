---
title: 无缝 SSO 用户登录问题
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2021
ms.locfileid: "49919197"
---
# <a name="seamless-sso-user-sign-in-issues"></a><span data-ttu-id="d972a-102">无缝 SSO 用户登录问题</span><span class="sxs-lookup"><span data-stu-id="d972a-102">Seamless SSO user sign-in issues</span></span>

<span data-ttu-id="d972a-103">对用户进行身份验证后，浏览器将缓存用户的凭据，以便在同一浏览器中，应用程序将自动使用同一帐户登录。</span><span class="sxs-lookup"><span data-stu-id="d972a-103">After the user is authenticated, the browser will cache the user's credentials, so that on the same browser, the application will automatically sign-in with the same account.</span></span> <span data-ttu-id="d972a-104">这可能会导致另一个用户或单个用户难以登录到一台设备上的多个帐户。</span><span class="sxs-lookup"><span data-stu-id="d972a-104">This may make it difficult for another user or a single user to log into multiple accounts on one device.</span></span> <span data-ttu-id="d972a-105">若要解决此问题：1.</span><span class="sxs-lookup"><span data-stu-id="d972a-105">To solve this: 1.</span></span> <span data-ttu-id="d972a-106">尝试在另一个浏览器上登录。</span><span class="sxs-lookup"><span data-stu-id="d972a-106">Try signing in on another browser.</span></span> <span data-ttu-id="d972a-107">2.</span><span class="sxs-lookup"><span data-stu-id="d972a-107">2.</span></span> <span data-ttu-id="d972a-108">清除浏览器的缓存和/或 Cookie，然后再次尝试登录。</span><span class="sxs-lookup"><span data-stu-id="d972a-108">Clear the browser's cache and/or cookies and try signing in again.</span></span>

<span data-ttu-id="d972a-109">如果仍遇到登录问题，我们建议执行下列操作来诊断和自动执行解决方案步骤：</span><span class="sxs-lookup"><span data-stu-id="d972a-109">If you are still experiencing sign-in issues, we recommend the following to diagnose and automate the resolution steps:</span></span>

1. <span data-ttu-id="d972a-110">安装 ["我的应用](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) "安全浏览器扩展，以帮助 Azure Active Directory (Azure AD) ，以在使用 Azure 门户中的测试体验时提供更好的诊断和解决方案。</span><span class="sxs-lookup"><span data-stu-id="d972a-110">Install the [My Apps Secure Browser Extension](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) to help Azure Active Directory (Azure AD) to provide better diagnosis and resolutions when using the testing experience in the Azure portal.</span></span>
2. <span data-ttu-id="d972a-111">在 Azure 门户的应用配置页面中使用测试体验重现错误。</span><span class="sxs-lookup"><span data-stu-id="d972a-111">Reproduce the error using the testing experience in the app configuration page in the Azure portal.</span></span> <span data-ttu-id="d972a-112">若要了解更多信息，请参阅 [调试基于 SAML 的单一登录应用程序](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)。</span><span class="sxs-lookup"><span data-stu-id="d972a-112">To learn more, see [Debug SAML-based single sign-on applications](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues).</span></span>
3. <span data-ttu-id="d972a-113">如果你将 Azure 门户中的测试体验与"我的应用"安全浏览器扩展一同使用，可以跳过步骤 **4。**</span><span class="sxs-lookup"><span data-stu-id="d972a-113">If you use the testing experience in the Azure portal with the My Apps Secure Browser Extension, you can **skip step 4**.</span></span>
4. <span data-ttu-id="d972a-114">若要打开基于 SAML 的单一登录配置页面：</span><span class="sxs-lookup"><span data-stu-id="d972a-114">To open the SAML-based single sign-on configuration page:</span></span>
    - <span data-ttu-id="d972a-115">打开 [Azure 门户](https://portal.azure.com/)，以全局管理员 **或\*\*\*\*Coadmin 登录**。</span><span class="sxs-lookup"><span data-stu-id="d972a-115">Open the [Azure portal](https://portal.azure.com/) and sign in as a **Global Administrator** or **Coadmin**.</span></span>
    - <span data-ttu-id="d972a-116">通过选择 **左侧主导航** 菜单顶部的"所有服务"打开 Azure Active Directory 扩展。</span><span class="sxs-lookup"><span data-stu-id="d972a-116">Open the **Azure Active Directory Extension** by selecting **All services** at the top of the main left-side navigation menu.</span></span>
    - <span data-ttu-id="d972a-117">在筛选器搜索框中键入"Azure Active Directory"，然后选择 **Azure Active Directory** 项。</span><span class="sxs-lookup"><span data-stu-id="d972a-117">Type "Azure Active Directory" in the filter search box and select the **Azure Active Directory** item.</span></span>
    - <span data-ttu-id="d972a-118">从 **Azure** Active Directory 左侧导航菜单中选择企业应用程序。</span><span class="sxs-lookup"><span data-stu-id="d972a-118">Select **Enterprise Applications** from the Azure Active Directory left-hand navigation menu.</span></span>
    - <span data-ttu-id="d972a-119">选择 **"所有** 应用程序"以查看所有应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="d972a-119">Select **All Applications** to view a list of all your applications.</span></span> <span data-ttu-id="d972a-120">如果在此处看不到要显示的应用程序，请使用"所有应用程序"列表顶部的筛选器控件，将"显示"选项设置为"**所有应用程序"。** </span><span class="sxs-lookup"><span data-stu-id="d972a-120">If you do not see the application you want show up here, use the **Filter** control at the top of the **All Applications List** and set the **Show** option to **All Applications**.</span></span>
    - <span data-ttu-id="d972a-121">选择要为单一登录配置的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d972a-121">Select the application you want to configure for single sign-on.</span></span>
    - <span data-ttu-id="d972a-122">加载应用程序后，从应用程序的左侧导航菜单中选择"单一登录"。</span><span class="sxs-lookup"><span data-stu-id="d972a-122">After the application loads, select **Single sign-on** from the application’s left-hand navigation menu.</span></span>
    - <span data-ttu-id="d972a-123">选择 **基于 SAML 的 SSO。**</span><span class="sxs-lookup"><span data-stu-id="d972a-123">Select **SAML-based SSO**.</span></span>
5. <span data-ttu-id="d972a-124">根据该错误，若要了解有关要遵循的建议步骤的详细信息，请参阅"登录到基于 SAML 的单一[登录配置的应用时遇到问题"。](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)</span><span class="sxs-lookup"><span data-stu-id="d972a-124">Based on the error, to learn more about the recommended steps to follow, see [Problems signing in to SAML-based single sign-on configured apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory).</span></span>
6. <span data-ttu-id="d972a-125">若要解决其他用户的登录问题，请参阅以下指南：</span><span class="sxs-lookup"><span data-stu-id="d972a-125">To troubleshoot other user sign-issues refer to the following guidance:</span></span>
    - [<span data-ttu-id="d972a-126">单Sign-On SAML 协议</span><span class="sxs-lookup"><span data-stu-id="d972a-126">Single Sign-On SAML protocol</span></span>](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [<span data-ttu-id="d972a-127">如何：使用 Azure Active Directory 报告排查登录错误</span><span class="sxs-lookup"><span data-stu-id="d972a-127">How to: Troubleshoot sign-in errors using Azure Active Directory reports</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [<span data-ttu-id="d972a-128">意外同意提示</span><span class="sxs-lookup"><span data-stu-id="d972a-128">Unexpected consent prompt</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [<span data-ttu-id="d972a-129">用户同意错误</span><span class="sxs-lookup"><span data-stu-id="d972a-129">User consent error</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [<span data-ttu-id="d972a-130">从"我的应用程序"登录时出现问题</span><span class="sxs-lookup"><span data-stu-id="d972a-130">Problems signing in from My Apps</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [<span data-ttu-id="d972a-131">应用程序登录页上的错误</span><span class="sxs-lookup"><span data-stu-id="d972a-131">Error on application sign-in page</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [<span data-ttu-id="d972a-132">登录 Microsoft App 时出现问题</span><span class="sxs-lookup"><span data-stu-id="d972a-132">Problem signing into a Microsoft App</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
