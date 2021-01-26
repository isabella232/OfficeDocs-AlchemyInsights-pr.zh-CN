---
title: 身份验证问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976839"
---
# <a name="authentication-issues"></a>身份验证问题

**查找关于从 Azure Active Directory (Azure AD) 安全令牌服务 (STS) 返回的 AADSTS 错误代码的信息？** 请参阅 [Azure AD 身份验证和授权错误代码](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 以查找 AADSTS 错误说明、修复和一些建议的解决方法。

授权错误可能是由多个不同的问题造成的，其中大多数问题会产生 401 或 403 错误。 例如，以下问题可能会导致授权错误：

- 不正确的[访问令牌获取流](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- 配置不当的[权限范围](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- 缺乏[许可](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent)

若要解决常见授权错误，请尝试执行以下与你遇到的错误最接近的步骤。 可能有多个步骤适用于你所遇到的某个错误。

**401 未授权错误：你的令牌是否有效？**

请确保应用在请求中向 Microsoft Graph 提供有效的访问令牌。 此错误通常意味着 HTTP 身份验证请求标头中缺少访问令牌，或者令牌无效或已过期。 强烈建议使用 Microsoft 身份验证库 (MSAL) 获取访问令牌。 此外，如果尝试使用授予个人 Microsoft 帐户的委派访问令牌来访问仅支持工作或学校帐户（组织帐户）的 API，也可能会发生此错误。

**403 禁止错误：你是否选择了正确的权限集？**

确保根据应用调用的 Microsoft Graph API 来请求正确的权限集。 所有 Microsoft Graph API 参考方法主题中都提供了我们建议的最低特权权限。 此外，这些权限必须由用户或管理员向应用程序授予。 授予权限通常通过同意页面进行，也可使用 Azure 门户应用程序注册边栏选项卡授予进行。 从应用程序的“**设置**”边栏选项卡，单击“**所需权限**”，然后单击“**授予权限**”。 有关详细信息，请参阅：

- [Microsoft Graph 权限](https://docs.microsoft.com/graph/permissions-reference) 
- [了解 Azure AD 权限和许可](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 禁止错误：你的应用是否获取了与所选权限匹配的令牌？**

确保请求或授予的权限类型与应用获取的访问令牌类型相匹配。 你可能正在请求和授予应用权限，但使用的是委派交互式代码流令牌，而不是客户端凭据流令牌，或者正在请求和授予委派权限，但使用的是客户端凭据流令牌，而不是委派代码流令牌。

有关于获取令牌相关的详细信息，请参阅：

- [代表用户获取访问权限和委派权限](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 - OAuth 2.0 授权代码流](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [在没有用户的情况下获取访问权限（守护程序服务）和应用程序权限](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 - OAuth 2.0 客户端凭据流](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 禁止访问错误：重置密码**

目前，没有应用程序权限守护程序服务到服务权限允许重置用户密码。 这些 API 仅支持对登录的管理员使用交互式委派代码流。 有关详细信息，请参阅 [Microsoft Graph 权限](https://docs.microsoft.com/graph/permissions-reference)。

**403 禁止：用户是否具有访问权限，是否获得许可？**

对于委派代码流，Microsoft Graph 将根据向应用授予的权限以及登录用户具有的权限来评估是否允许请求。 通常，此错误表示用户没有足够的特权执行请求 **或者** 用户没有获得所访问数据的许可。 只有具有所需权限或许可证的用户才能成功发出请求。

**403 禁止：是否选择了正确的资源 API？**

API 服务（如 Microsoft Graph）检查接收的访问令牌中的 *aud* 声明 (audience) 是否与其本身的预期值匹配，如果不匹配，则会出现 403 禁止错误。 导致此错误的常见错误是尝试使用为 Azure AD Graph API、Outlook API 或 SharePoint/OneDrive API 获取的令牌调用 Microsoft Graph（或反之）。 确保你的应用为其获取令牌的资源（或范围）与应用调用的 API 匹配。

**400 错误请求或 403 禁止：用户是否符合其组织的条件访问 (CA) 策略？**

根据组织的条件访问 (CA) 策略，通过你的应用访问 Microsoft Graph 资源的用户可能会被要求提供附加信息，而这些信息在应用最初获取的访问令牌中并不存在。 在这种情况下，你的应用在获取访问令牌期间会收到 **400 以及 *interaction_required*** 错误，或者在调用 Microsoft Graph 时收到 **403 以及 *insufficient_claims*** 错误。 在这两种情况下，错误响应都包含可呈现给授权终结点的附加信息，以便要求用户提供其他信息（如多重身份验证或设备注册）。

有关条件访问相关的详细信息，请参阅：

- [使用 MSAL 处理条件访问质询](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Azure Active Directory 条件访问开发人员指南](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_对 Azure Active Directory 身份验证库 (ADAL) 和 Azure AD Graph API (AAD Graph) 的支持终止_* _

- 自 2020 年 6 月 30 日起，我们将不再向 Azure Active Directory 身份验证库 (ADAL) 和 Azure AD Graph API (AAD Graph) 添加任何新功能。 我们将继续提供技术支持和安全更新，但不再提供功能更新。
- 自 2022 年 6 月 30 日起，我们将终止对 ADAL 和 Azure AD Graph 的支持，并且将不再提供技术支持或安全更新。
    - 此时间之后，在现有 OS 版本上使用 ADAL 的应用将继续工作，但将不会获得任何技术支持或安全更新。
    - 此时间之后，使用 Azure AD Graph 的应用将不再接收来自 AAD Graph 终结点的响应。

_ *ADAL 迁移**

我们建议更新到具有最新功能和安全更新的 [Microsoft 身份验证库 (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)。 此建议是在 Microsoft 在支持结束截止期限之前将其应用程序迁移到 MSAL 的背景下提出的。 Microsoft 应用向 MSAL 迁移的目标时确保应用能够从 MSAL 的持续安全和功能改进中获益。

- [请阅读 ADAL 常见问题解答](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [了解在不同平台上如何迁移应用](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- 如果在了解哪些应用使用 ADAL 方面需要帮助，我们建议查看应用的全部源代码，如果适用，还请联系任何独立软件供应商 (ISV) 或应用提供商。 Microsoft 支持部门也可提供租户内所有非 Microsoft ADAL 应用的列表。

**AAD Graph 迁移**

对于使用 AAD Graph 的应用程序，请按照我们关于 [迁移 Azure AD Graph 应用到 Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true) 的指南操作。

- [我们的迁移清单提供了入门起点](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。 
- 你的 Azure 应用注册门户显示了哪些应用正在使用 AAD Graph。 我们建议查看应用的全部源代码，并且如果适用，请联系任何 ISV 或应用提供商。 Microsoft 支持部门也可提供租户内所有 AAD Graph 使用情况的信息。

 










