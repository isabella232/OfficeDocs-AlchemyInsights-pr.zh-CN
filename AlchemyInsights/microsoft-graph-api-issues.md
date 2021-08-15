---
title: Microsoft Graph API 问题
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
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975883"
---
# <a name="microsoft-graph-api-issues"></a>Microsoft Graph API 问题

本主题还适用于仍在使用 Azure AD Graph API 的开发人员。 但是，**强烈建议** 将 Microsoft Graph用于所有目录、标识和访问管理方案。

**身份验证或授权问题**

- 如果你的应用无法获取调用 Microsoft Graph 的令牌，请选择"获取访问令牌 **的问题 (身份验证)** Microsoft Graph"类别，获取有关本主题的更具体的帮助和支持。
- 如果你的应用在调用 Microsoft Graph 时收到 **401 或 403** 授权错误，请选择"获取访问被拒绝错误 **(授权)** Microsoft Graph API"类别，获取有关本主题的更具体的帮助和支持。

**我想要使用 Microsoft Graph，但不确定从何处开始**

- [Microsoft Graph 概述](https://docs.microsoft.com/graph/overview)
- [Microsoft 服务中的标识和访问管理Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [开始构建 Microsoft Graph应用](https://docs.microsoft.com/graph/)
- **Microsoft Graph资源管理器**- Graph租户或演示租户中测试 Microsoft api

**我想要使用 Microsoft Graph，但它是否支持所需的 v1.0 目录 API？**

Microsoft Graph 是推荐的用于目录、标识和访问管理的 API。 但是，Azure AD 应用程序与 Microsoft Graph 之间仍有一些Graph。 查看以下文章，这些文章重点介绍了可帮助你做出选择的最最新差异：

- [Azure AD 应用程序与 Microsoft Graph 之间的资源类型Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD Graph 和 Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD 和 Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**我调用的 API 不起作用 - 在哪里可以执行更多测试？**

**Microsoft Graph资源管理器**- 在租户或演示租户中测试 Microsoft Graph API，并查看 Microsoft Graph资源管理器中的示例查询。

**我的应用过慢，并且也受到限制。我可以进行哪些改进？**

根据你的方案，有多种选项可供选择，使应用程序性能更高;在某些情况下，当您在) 中执行过多调用时，服务 (很容易受到限制。

- [Microsoft Graph最佳实践](https://docs.microsoft.com/graph/best-practices-concept)
- [批处理请求](https://docs.microsoft.com/graph/json-batching)
- [通过 delta 查询跟踪更改](https://docs.microsoft.com/graph/delta-query-overview)
- [通过 Webhook 获取更改通知](https://docs.microsoft.com/graph/webhooks)
- [限制指南](https://docs.microsoft.com/graph/throttling)

**在哪里可以找到有关错误和已知问题的详细信息？**

- [Microsoft Graph错误响应信息](https://docs.microsoft.com/graph/errors)
- [Microsoft Graph 已知问题](https://docs.microsoft.com/graph/known-issues)

**在哪里可以检查服务可用性和连接状态？**

可通过 Microsoft 服务访问的基础服务的服务可用性和连接Graph Microsoft 服务的整体可用性和性能Graph。

- For Azure Active Directory service health， check the status of **Security + Identity** services listed in the Azure status [page](https://azure.microsoft.com/status/).
- 对于Office Microsoft 服务Graph，请检查服务运行状况仪表板中Office[服务的状态](https://portal.office.com/adminportal/home#/servicehealth)。

Microsoft Graph授权错误可能是多个不同问题的结果，其中大多数问题都生成 401 或 403 错误。 例如，以下情况可能会导致授权错误：

- 不正确的[访问令牌获取流](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- 配置不当的[权限范围](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- 缺乏[许可](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***停止支持 ADAL Azure Active Directory ADAL (和 Azure AD) API Graph AAD (AAD Graph)***

**从 2020** 年 6 月 30 日开始，我们将不再将任何新功能添加到 ADAL 和 Azure AD Graph。 我们将继续提供技术支持和安全更新，但不再提供功能更新。

**从 2022** 年 6 月 30 日开始，我们将停止对 ADAL 和 Azure AD Graph将不再提供技术支持或安全更新。

此时间之后，在现有 OS 版本上使用 ADAL 的应用将继续工作，但将不会 *获得任何技术支持或安全更新*。

此后，使用 Azure AD Graph 的应用可能不再接收来自 Azure AD Graph 端点的响应。

**ADAL 迁移**

我们建议更新到具有最新功能和安全更新的 [Microsoft 身份验证库 (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)。

如果你使用的是 Microsoft 应用，请了解 Microsoft 正在将应用程序迁移到 MSAL，到支持期限结束，确保他们将受益于 MSAL 正在进行的安全和功能改进。

1. [请阅读 ADAL 常见问题解答](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [了解如何在不同平台上迁移应用](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. 如果你需要了解哪些应用使用 ADAL 的帮助，我们建议你查看所有应用的源代码，如果适用，请联系任何 ISV 或应用提供商。 Microsoft 支持部门也可提供租户内所有非 Microsoft ADAL 应用的列表。

**AAD Graph 迁移**

对于使用 Azure AD Graph，请按照我们的指南将 Azure [AD Graph应用迁移到 Microsoft Graph。](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [我们的迁移清单提供了入门起点](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。
2. 你的 Azure 应用注册门户显示了哪些应用正在使用 AAD Graph。 我们建议查看应用的全部源代码，并且如果适用，请联系任何 ISV 或应用提供商。 Microsoft 支持还可以提供租户中所有 AAD Graph列表。
3. 若要使你的应用可访问 Microsoft Graph 中的数据，用户或管理员必须通过同意过程向其授予正确的权限。 [Microsoft Graph权限](https://docs.microsoft.com/graph/permissions-reference)参考列出了与每个主要 Microsoft 应用程序 API 集Graph的权限。 它还提供有关如何使用权限的指导。
