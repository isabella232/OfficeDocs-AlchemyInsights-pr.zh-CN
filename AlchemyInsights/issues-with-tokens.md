---
title: 令牌问题
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
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49911983"
---
# <a name="issues-with-tokens"></a>令牌问题

要管理与令牌相关的问题，可以执行以下步骤：

1. 您可以指定由 Microsoft 标识平台颁发的访问、ID 或 SAML 令牌的生存期。 可以为组织中的所有应用程序、多租户（多组织）应用程序或组织中的特定服务主体设置令牌生存期。 有关详细信息，请参阅[Microsoft 标识平台中的可配置令牌生存期（预览）](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。
2. 访问令牌使客户端能够安全地调用受保护的 Web API，并被 Web API 用来执行身份验证和授权。 根据 OAuth 规范，访问令牌是没有设置格式的不透明字符串 — 一些标识提供者 (IDP) 使用 GUID，另一些使用加密 blob。 Microsoft 标识平台使用多种访问令牌格式，具体取决于接受令牌的 API 的配置。 要了解 API 如何验证和使用访问令牌内的声明，请参阅 [Microsoft 标识平台访问令牌](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint)。
3. Microsoft 身份验证库 (MSAL) 支持在不同应用程序方案中使用的多个身份验证流。 有关更多信息，请参阅[身份验证流](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes)。
4. OAuth2.0 授权代码授权可用于安装在设备上的应用程序，以访问受保护的资源，如 Web API。 使用 OAuth 2.0 的 Microsoft 标识平台实现，可以向移动和桌面应用程序添加登录和 API 访问。 请参阅 [Microsoft 标识平台和 OAuth 2.0 授权代码流](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token)，了解如何使用任何语言直接对应用程序中的协议进行编程。
5. OpenID 连接 (OIDC) 是构建在 oauth2.0 上的身份验证协议，可以使用它安全地将用户登录到应用程序。 使用 Microsoft 标识平台端点的 OpenID 连接实现时，可以向应用程序添加登录和 API 访问。 [Microsoft 标识平台和 OpenID 连接协议](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request)演示了如何独立于语言进行此操作，并描述了如何在不使用任何 Microsoft 开放源代码库的情况下发送和接收 HTTP 消息。
    - 用户信息端点是 OIDC 标准的一部分，旨在返回有关已验证用户的声明。 有关详细信息，请参阅 [Microsoft 标识平台用户信息端点](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead)。
    - [使用 Azure AD 和 OpenID 连接在 web 应用程序中调用 Web API](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) 示例显示如何构建 MVC Web 应用程序，该应用程序使用 OpenID 连接协议以使用 Azure AD 进行登录，然后使用通过 OAuth 2.0 获得的令牌在登录用户的身份下调用 Web API。 本示例使用 OpenID Connect ASP .Net OWIN 中间件和 ADAL .Net。
6. [配置应用程序以公开 Web API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) — 在此快速入门中，可以向 Microsoft 标识平台注册 Web API，并通过添加示例范围将其公开给客户端应用程序。 通过注册 Web API 并通过作用域公开它，可以向访问你的 API 的授权用户和客户端应用程序提供对其资源的基于权限的访问。
7. 在 Azure Active Directory B2C (Azure AD B2C) 中，资源所有者密码凭据 (ROPC) 流是 OAuth 标准身份验证流。 在此流中，应用程序（也称为信赖方）为令牌交换有效凭据。 凭据包括用户 ID 和密码。 返回的令牌是 ID 令牌、访问令牌和刷新令牌。 有关更多信息，请参阅[在 Azure Active Directory B2C 中设置资源所有者密码凭据流](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow)。 

