---
title: 链接和 URL 的问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: d85069970fe6bc6cc7a8488c49c0e6236426d45b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321897"
---
# <a name="issues-with-links-and-urls"></a>链接和 URL 的问题

重定向 URI/答复 URL（两个表达式可以互换）是 Microsoft 身份平台用于返回应用请求的令牌的 URL。有关这些 URL 的信息，请参阅以下文章：

- [身份验证流和应用程序方案](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - 有关每个方案 **应用注册** 页面中重定向 URI 的信息。
- [重定向 URI/答复 URL 限制和限度](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**我不知道如何为我的应用注册正确的重定向 URI/答复 URL**

使用正在开发的应用程序登录时，如果登录对话框显示 **AADSTS50011：请求中指定的答复 URL 与为应用程序 <your app ID>** 配置的答复 URL 不匹配，你需要向你的应用程序注册添加重定向 URI（即代码在向 Microsoft 身份平台的令牌请求中所使用的重定向 URI）。

若要添加答复 URL，请转到 Azure 门户中 **应用程序注册** 页面中的 **身份验证** 选项卡，在 “**重定向 URL**”部分中添加一个条目。 需要输入的值取决于正在构建的应用程序类型，如下所述：

- 对于单页应用程序和 Web 应用，答复 URL 就是应用程序中的 URL。 请参阅 [单页应用程序注册](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri) 或 [使用 Azure 门户注册 web 应用型应用](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- 对于桌面应用，需要选择的值取决于：
    - 平台（MacOS 不同于 Windows 或 Linux）
    - 获取令牌的方式（交互式、使用设备代码流、使用集成 Windows 身份验证 [IWA] 或者通过用户名/密码）。
    有关详细信息，请参阅 [桌面应用 - 应用注册 - 重定向 URi](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- 对于移动应用程序，重定向 URI 取决于：
    - 平台 (iOS/Android/UWP)
    - 用于生成应用的信息（例如 iOS 中的捆绑 ID）以及 Android 上的包名称和签名哈希。Azure 门户应用注册将帮助你。有关详细信息，请参阅[平台配置和重定向 URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris)。

**注意**：Web API 和一些获取令牌（IWA 和用户名/密码）的无提示方式不需要重定向 URI。

**我已部署 Web 应用程序，但测试已部署的应用时，收到答复 URL 不匹配的消息**

为部署 Web 应用程序的所有位置添加重定向 URI。 有关详细信息，请参阅 [使用 Azure 门户注册 Web 应用型应用](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)。

**注意**：在将应用程序部署到某个位置后，立即添加该位置的重定向 URI。

**我无法注册足够的答复 URL**

你是 ISV 用户，而且你的每个客户具有一个或多个重定向 URI。 你希望从 ADAL/Azure AD v1.0 迁移到 MSAL/Microsoft 标识平台，并点击 [重定向 URL 的最大数目](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris)。 若要解决此问题，对于与每个客户相应的服务主体，[向其添加重定向 URI](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals)。
