---
title: OAuth 2.0和OpenID Connect协议的排除故障。
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: 7584d8f6f2e24812c1fdded76332edc6dd671034011e262c15756567cb467c26
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921033"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>OAuth 2.0和OpenID Connect协议的排除故障。

要解决 OAuth 2.0 和 OpenID Connect 问题，请执行以下建议步骤：

请参阅下列与 OAuth 2.0 和 OpenID Connect 协议的配置和疑难解答相关的文章：

- [Microsoft 标识平台和 OAuth 2.0 授权代码流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) - 本文介绍如何使用任意语言直接针对应用程序中的 **代码授予(PKCE)流程** 进行编程。
- [Microsoft 标识平台和 OAuth 2.0 客户端凭据流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) - 本文介绍如何直接针对应用程序中的 **客户端凭据流程** 进行编程。
- [Microsoft 标识平台和 OAuth 2.0 资源所有者密码凭据](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) - 本文介绍如何直接针对应用程序中的 **ROPC 流程** 进行编程。
    - Microsoft 标识平台仅支持适用于 Azure AD 租户的 ROPC，而并不支持个人帐户。 这意味着必须使用租户特定的端点 **（https://login.microsoftonline.com/{TenantId_or_Name})** 或 **组织** 的端点。
    - 受邀到 Azure AD 租户的个人帐户不能使用 ROPC。
    - 没有密码的帐户不能通过 ROPC 登录。 对于这种情况，我们建议你为应用使用不同的流程。
    - 如果用户需要通过 [多种身份验证 (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) 登录到应用程序,用户将被阻止。
    - 混合联合身份验证 [方案](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) （例如，用于对本地帐户进行身份验证的 Azure AD 和 ADFS）不支持 ROPC。 如果将用户重定向到本地身份提供程序的完整页面，Azure AD 无法针对该身份提供程序测试用户名和密码。 但是，ROPC 支持[通过式身份验证](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) 。
    - 混合联合身份验证方案的例外是：将 **AllowCloudPasswordValidation** 设置为 **TRUE** 的主领域发现策略将允许 ROPC flow 在本地密码同步到云时，为联合用户工作。 有关详细信息，请参阅 [旧版应用程序启用联合用户的直接 ROPC 身份验证](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Microsoft 标识平台和 OAuth 2.0 代表流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) - 本文介绍如何直接针对应用程序中的 **代表 (OBO) 流程** 进行编程。
- [Microsoft 标识平台和 OpenID Connect 协议](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc)- 本文展示了如何实现独立于语言的OpenID Connect协议 ，并介绍了在不实用任何 Microsoft 开放源代码库的情况下发送和接收 HTTP 消息。

**访问令牌**

要了解 API 如何验证和使用访问令牌内的声明，请参阅 [Microsoft 标识平台访问令牌](https://docs.microsoft.com/azure/active-directory/develop/access-tokens)。 本文中除记录外的所有文档都仅适用于已注册的 API 所发布的令牌。 此令牌不适用于为 Microsoft 拥有的 API 发布的令牌，也不能用这些令牌来验证 Microsoft 标识平台将如何为所创建的 API 发布令牌。

**应用程序配置**

[重定向 URI（答复 URL）限制](https://docs.microsoft.com/azure/active-directory/develop/reply-url) - 了解如何配置重定向 URI（答复 URL）。 重定向 URI 或答复 URL 是授权服务器在应用成功授权并授予用户授权代码或访问令牌后向用户发送的位置。 授权服务器会将代码或令牌发送到重定向 URI;因此，在应用注册过程中必须注册正确的位置。

**应用程序设置**

[教程：为SCIM端点开发和计划设置](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) - 本文介绍如何构建 SCIM 端点和集成 AAD 设置服务。


