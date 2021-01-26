---
title: 链接和 URL 的问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950688"
---
# <a name="issues-with-links-and-urls"></a><span data-ttu-id="2c152-102">链接和 URL 的问题</span><span class="sxs-lookup"><span data-stu-id="2c152-102">Issues with links and URLs</span></span>

<span data-ttu-id="2c152-103">重定向 URI/答复 URL（两个表达式可以互换）是 Microsoft 身份平台用于返回应用请求的令牌的 URL。</span><span class="sxs-lookup"><span data-stu-id="2c152-103">Redirect URI/reply URLs (both expressions are interchangeable) are the URLs used by the Microsoft identity platform to return app-requested tokens.</span></span> <span data-ttu-id="2c152-104">有关这些 URL 的信息，请参阅以下文章：</span><span class="sxs-lookup"><span data-stu-id="2c152-104">For information on these URLs, see the following articles:</span></span>

- <span data-ttu-id="2c152-105">[身份验证流和应用程序方案](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - 有关每个方案 **应用注册** 页面中重定向 URI 的信息。</span><span class="sxs-lookup"><span data-stu-id="2c152-105">[Authentication flows and application scenarios](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - Information about the redirect URIs in the **App registration** page for each scenario.</span></span>
- [<span data-ttu-id="2c152-106">重定向 URI/答复 URL 限制和限度</span><span class="sxs-lookup"><span data-stu-id="2c152-106">Redirect URI/reply URL restrictions and limitations</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

<span data-ttu-id="2c152-107">**我不知道如何为我的应用注册正确的重定向 URI/答复 URL**</span><span class="sxs-lookup"><span data-stu-id="2c152-107">**I don't know how to register the right redirect URI / reply URL for my app**</span></span>

<span data-ttu-id="2c152-108">使用正在开发的应用程序登录时，如果登录对话框显示 **AADSTS50011：请求中指定的答复 URL 与为应用程序 <your app ID>** 配置的答复 URL 不匹配，你需要向你的应用程序注册添加重定向 URI（即代码在向 Microsoft 身份平台的令牌请求中所使用的重定向 URI）。</span><span class="sxs-lookup"><span data-stu-id="2c152-108">When you sign in with the application you are developing, if the sign-in dialog displays **AADSTS50011: The reply url specified in the request does not match the reply urls configured for the application <your app ID>**, you'll need to add to your application registration, the redirect URI that your code used in the token request to the Microsoft identity platform.</span></span>

<span data-ttu-id="2c152-109">若要添加答复 URL，请转到 Azure 门户中 **应用程序注册** 页面中的 **身份验证** 选项卡，在 “**重定向 URL**”部分中添加一个条目。</span><span class="sxs-lookup"><span data-stu-id="2c152-109">To add a reply URL, go to the **Authentication** tab in your **application registration** page in the Azure portal and add an entry in the **Redirect URIs** section.</span></span> <span data-ttu-id="2c152-110">键入重定向 URL（Web 或移动/桌面）。</span><span class="sxs-lookup"><span data-stu-id="2c152-110">Redirect URIs are typed (Web or mobile/desktop).</span></span> <span data-ttu-id="2c152-111">需要输入的值取决于正在构建的应用程序类型，如下所述：</span><span class="sxs-lookup"><span data-stu-id="2c152-111">The value you need to enter depends on the type of application you're building, as described below:</span></span>

- <span data-ttu-id="2c152-112">对于单页应用程序和 Web 应用，答复 URL 就是应用程序中的 URL。</span><span class="sxs-lookup"><span data-stu-id="2c152-112">For single-page applications and web apps, the reply URL is a URL in your application.</span></span> <span data-ttu-id="2c152-113">请参阅 [单页应用程序注册](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) 或 [使用 Azure 门户注册 web 应用型应用](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="2c152-113">See [Single-page application registration](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) or [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)</span></span>
- <span data-ttu-id="2c152-114">对于桌面应用，需要选择的值取决于：</span><span class="sxs-lookup"><span data-stu-id="2c152-114">For desktop apps, the value that you need to choose depends on:</span></span>
    - <span data-ttu-id="2c152-115">平台（MacOS 不同于 Windows 或 Linux）</span><span class="sxs-lookup"><span data-stu-id="2c152-115">the platform (MacOS is different from Windows or Linux)</span></span>
    - <span data-ttu-id="2c152-116">获取令牌的方式（交互式、使用设备代码流、使用集成 Windows 身份验证 [IWA] 或者通过用户名/密码）。</span><span class="sxs-lookup"><span data-stu-id="2c152-116">the way you acquire the token (interactively, with device code flow, with Integrated Windows Authentication [IWA] or with username/password).</span></span>
    <span data-ttu-id="2c152-117">有关详细信息，请参阅 [桌面应用 - 应用注册 - 重定向 URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span><span class="sxs-lookup"><span data-stu-id="2c152-117">For details, see [Desktop apps - App registration - Redirect URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)</span></span>
- <span data-ttu-id="2c152-118">对于移动应用程序，重定向 URI 取决于：</span><span class="sxs-lookup"><span data-stu-id="2c152-118">For mobile applications, the redirect URI depends on:</span></span>
    - <span data-ttu-id="2c152-119">平台 (iOS/Android/UWP)</span><span class="sxs-lookup"><span data-stu-id="2c152-119">the platform (iOS/Android/UWP)</span></span>
    - <span data-ttu-id="2c152-120">构建应用时所使用的信息（如 iOS 中的捆绑 ID，以及 Android 上的包名称和签名哈希）。Azure 门户应用注册将有所帮助。</span><span class="sxs-lookup"><span data-stu-id="2c152-120">the information used to build your app, such as the bundle ID in iOS, and the package name and signature hash on Android The Azure portal app registration will help you.</span></span> <span data-ttu-id="2c152-121">有关详细信息，请参阅 [平台配置和重定向 URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris)。</span><span class="sxs-lookup"><span data-stu-id="2c152-121">For details, see [Platform configuration and redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris).</span></span>

> [!NOTE]
> <span data-ttu-id="2c152-122">Web API 和获取令牌（IWA 和用户名/密码）的一些无提示方式不需要重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="2c152-122">Web APIs and some of the silent ways of acquiring tokens (IWA and username/password) don't require a redirect URI.</span></span>

<span data-ttu-id="2c152-123">**我已部署 Web 应用程序，但测试已部署的应用时，收到答复 URL 不匹配的消息**</span><span class="sxs-lookup"><span data-stu-id="2c152-123">**I've deployed my web application and when I test the deployed app, I get a reply url mismatch message**</span></span>

<span data-ttu-id="2c152-124">为部署 Web 应用程序的所有位置添加重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="2c152-124">Add redirect URIs for all the locations at which you are deploying your web application.</span></span> <span data-ttu-id="2c152-125">有关详细信息，请参阅 [使用 Azure 门户注册 Web 应用型应用](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)。</span><span class="sxs-lookup"><span data-stu-id="2c152-125">For more information, see [Register a web app app using Azure portal](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration).</span></span>

> [!NOTE]
> <span data-ttu-id="2c152-126">在将应用程序部署到某个位置后，立即为该位置添加重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="2c152-126">Add redirect URI for a location immediately after you have deployed the application at that location.</span></span>

<span data-ttu-id="2c152-127">**我无法注册足够的答复 URL**</span><span class="sxs-lookup"><span data-stu-id="2c152-127">**I can't register enough reply URLs**</span></span>

<span data-ttu-id="2c152-128">你是 ISV 用户，而且你的每个客户具有一个或多个重定向 URI。</span><span class="sxs-lookup"><span data-stu-id="2c152-128">You're an ISV and have one or several redirect URIs for every customer of yours.</span></span> <span data-ttu-id="2c152-129">你希望从 ADAL/Azure AD v1.0 迁移到 MSAL/Microsoft 标识平台，并点击 [重定向 URL 的最大数目](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris)。</span><span class="sxs-lookup"><span data-stu-id="2c152-129">You want to migrate from ADAL/Azure AD v1.0 to MSAL/the Microsoft identity platform and you hit the [maximum number of redirect URIs](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris).</span></span> <span data-ttu-id="2c152-130">若要解决此问题，对于与每个客户相应的服务主体，[向其添加重定向 URI](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals)。</span><span class="sxs-lookup"><span data-stu-id="2c152-130">To resolve this, [add redirect URIs to service principals](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals) that correspond to each of your customers.</span></span>
