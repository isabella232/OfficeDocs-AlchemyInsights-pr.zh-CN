---
title: 解决基于 OIDC 的无缝单一登录 (SSO) 问题
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
- "9004357"
- "9375"
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50726912"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>解决基于 OIDC 的无缝单一登录 (SSO) 问题

- 若要了解如何将基于 OIDC 的应用添加到 Azure 租户，请参阅快速入门：为 [Azure Active Directory (Azure AD) ](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)租户中的应用程序设置基于 OIDC 的单一登录 (SSO) 。
- 有关使用 OpenID Connect 标准实现单一登录的应用的更多详细信息，请参阅了解基于 [OIDC 的单一登录](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)。
- 有关选择直接发送和处理 HTTP 请求或使用第三方开放源代码库（而不是使用其中一个开放源代码库）编写代码的信息，请参阅 Microsoft 标识平台上的 [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)和 OpenID Connect 协议。

**协议**

1. [Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) 标识平台和隐式授权流 - 隐式授予的定义特征是令牌 (ID 令牌或访问令牌) 直接从 /authorize 终结点而不是 /token 终结点返回。 这通常用作授权代码流的一部分，在所谓的"混合流"中 - 检索 /authorize 请求上的 ID 令牌 **以及授权代码**。 本文介绍如何直接针对应用程序中的协议进行编程，以从 Azure AD 请求令牌。
2. Microsoft 标识平台和[OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow)授权代码流 - OAuth 2.0 授权代码授予可用于安装在设备上的应用，以获得对受保护资源（如 Web API）的访问权限。 使用 OAuth 2.0 的 Microsoft 标识平台实现，你可以向移动和桌面应用添加登录和 **API 访问**。 本文介绍如何使用任意语言直接针对应用程序中的协议进行编程。
3. [Microsoft 标识平台和 OpenID Connect 协议](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) - 当你使用 Microsoft 标识平台的 OpenID Connect 实现时，你可以向应用添加登录和 API 访问。 本文介绍如何独立于语言执行这一操作，并介绍如何在没有任何 **Microsoft** 开放源代码库的情况下发送和接收 HTTP 消息。
4. Microsoft 标识平台和 [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)客户端凭据流 - 您可以使用 RFC 6749 中指定的 OAuth 2.0 客户端凭据（有时称为双行 **OAuth）** 使用应用程序的标识访问 Web 托管的资源。 这种类型的授予通常用于必须在后台运行的服务器到服务器交互，而无需与用户立即交互。 这些类型的应用程序通常称为守护 **程序** 或 **服务帐户**。 本文介绍如何直接针对应用程序中的协议进行编程。
