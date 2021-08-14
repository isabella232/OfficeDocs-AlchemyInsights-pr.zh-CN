---
title: 应用程序错误
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "7841"
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931439"
---
# <a name="application-errors"></a>应用程序错误

要查找有关从 STS Azure Active Directory (中的 Azure AD) 安全令牌服务 (**AADSTS**) ？ 阅读[Azure AD 身份验证](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes)和授权错误代码，以查找 AADSTS 错误描述、修补程序和一些建议的解决方法。

授权错误可能是由多个不同的问题造成的，其中大多数问题会产生 401 或 403 错误。 例如，以下情况可能会导致授权错误：

- 不正确的[访问令牌获取流](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- 配置不当的[权限范围](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- 缺乏[许可](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

若要解决常见的授权错误，请尝试下面提供的步骤，这些步骤与您收到的错误最匹配。 多个可能适用。

**401 未授权错误：你的令牌是否有效？**

确保应用程序在请求中向 Microsoft Graph有效的访问令牌。 此错误通常意味着 HTTP 身份验证请求标头中缺少访问令牌，或者令牌无效或已过期。 强烈建议使用 [Microsoft 身份验证库 (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) 获取访问令牌。 此外，如果你尝试使用授予个人 Microsoft 帐户的委派访问令牌访问仅支持工作或学校帐户或组织帐户的 API， (此错误) 。

**403 禁止错误：你是否选择了正确的权限集？**

检查你已基于应用调用的 Microsoft Graph API 请求了正确的权限集。 所有 Microsoft Graph API 参考方法主题中都提供了建议最低特权权限。 此外，这些权限必须由用户或管理员向应用程序授予。 授予权限通常通过同意页进行，也可使用 Azure 门户应用程序注册边栏选项卡授予权限。 从应用程序的“**设置**”边栏选项卡，单击“**所需权限**”，然后单击“**授予权限**”。

- [Microsoft Graph 权限](https://docs.microsoft.com/graph/permissions-reference) 
- [了解 Azure AD 权限和许可](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 禁止错误：你的应用是否获取了与所选权限匹配的令牌？**

确保请求或授予的权限类型与你的应用获取的访问令牌类型相匹配。 你可能正在请求和授予应用程序权限，但使用的是委派的交互式代码流令牌而不是客户端凭据流令牌，或者正在请求和授予委派权限，但使用的是客户端凭据流令牌而不是委派的代码流令牌。

- [代表用户获取访问权限和委派权限](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 - OAuth 2.0 授权代码流](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [在没有用户的情况下获取访问权限（守护程序服务）和应用程序权限](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 - OAuth 2.0 客户端凭据流](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 禁止访问错误：重置密码**

目前，没有应用程序权限守护程序服务到服务权限允许重置用户密码。 这些 API 仅支持对登录的管理员使用交互式委派代码流。

- [Microsoft Graph 权限](https://docs.microsoft.com/graph/permissions-reference)

**403 禁止：用户是否具有访问权限，是否获得许可？**

对于委托的代码流，Microsoft Graph根据授予应用的权限和登录用户拥有的权限来评估请求是否允许。 通常，此错误表示用户没有足够的特权执行请求或者用户没有获得所访问数据的许可。 只有具有所需权限或许可证的用户才能成功发出请求。

**403 禁止：是否选择了正确的资源 API？**

Api 服务（如 Microsoft Graph）检查收到的访问令牌中的 aud 声明 (受众) 是否与它本身预期的值匹配，如果未匹配，则会导致 403 禁止错误。 导致此错误的常见错误是尝试使用为 Azure AD Graph API、Outlook API 或 SharePoint/OneDrive API 获取的令牌调用 Microsoft Graph（或反之）。 确保你的应用为其获取令牌的资源（或范围）与应用调用的 API 匹配。

**400 错误请求或 403 禁止：用户是否符合其组织的条件访问 (CA) 策略？**

根据组织的 CA 策略，可能要求用户通过你的应用访问 Microsoft Graph 资源，获取最初获取的应用的访问令牌中未提供的其他信息。 在这种情况下，你的应用在获取访问令牌期间会收到 400 以及 *interaction_required* 错误，或者在调用 Microsoft Graph 时收到 403 以及 *insufficient_claims* 错误。 在这两种情况下，错误响应都包含可呈现给授权终结点的附加信息，以便向用户质询其他信息（如多重身份验证或设备注册）。

- [使用 MSAL 处理条件访问挑战 ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Azure Active Directory 条件访问开发人员指南](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
