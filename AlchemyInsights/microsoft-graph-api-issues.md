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
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/29/2021
ms.locfileid: "50716193"
---
# <a name="microsoft-graph-api-issues"></a>Microsoft Graph API 问题

本主题还适用于仍在使用 Azure AD Graph API 的开发人员。 但是， **强烈建议** 将 Microsoft Graph 用于所有目录、标识和访问管理方案。

**身份验证或授权问题**

- 如果你的应用无法获取令牌来调用 Microsoft Graph，请选择"获取访问令牌 (身份验证) Microsoft **Graph"** 类别以获取有关本主题的更具体的帮助和支持。
- 如果你的应用在调用 Microsoft Graph 时收到 **401 或 403** 授权错误，请选取"获取拒绝访问错误 **(授权)** Microsoft Graph API"类别，获取有关本主题的更具体的帮助和支持。

**我想要使用 Microsoft Graph，但不确定从何处开始**

- [Microsoft Graph 概述](https://docs.microsoft.com/graph/overview)
- [Microsoft Graph 中的标识和访问管理概述](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [构建 Microsoft Graph 应用入门](https://docs.microsoft.com/graph/)
- **Microsoft Graph 资源管理器** - 在租户或演示租户中测试 Microsoft Graph API

**我想要使用 Microsoft Graph，但它是否支持所需的 v1.0 目录 API？**

Microsoft Graph 是目录、标识和访问管理的推荐 API。 但是，Azure AD Graph 和 Microsoft Graph 中的可能功能之间仍有一些差异。 查看以下文章，其中重点介绍了最新的差异，以帮助你做出选择：

- [Azure AD Graph 和 Microsoft Graph 之间的资源类型差异](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD Graph 和 Microsoft Graph 之间的属性差异](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD 和 Microsoft Graph 之间的方法差异](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**我调用的 API 不起作用 - 在哪里可以执行更多测试？**

**Microsoft Graph 资源管理器**- 在租户或演示租户中测试 Microsoft Graph API，并查看 Microsoft Graph 资源管理器中的示例查询。 

**我的应用过慢，并且正被限制。我可以进行哪些改进？**

根据你的方案，有多种选项可供选择，使应用程序更具有性能;在某些情况下，当您对应用程序执行过多调用时，服务 (将不太容易) 。

- [Microsoft Graph 最佳做法](https://docs.microsoft.com/graph/best-practices-concept)
- [批处理请求](https://docs.microsoft.com/graph/json-batching)
- [通过增量查询跟踪更改](https://docs.microsoft.com/graph/delta-query-overview)
- [通过 Webhook 获取更改通知](https://docs.microsoft.com/graph/webhooks)
- [限制指南](https://docs.microsoft.com/graph/throttling)

**在哪里可以找到有关错误和已知问题的详细信息？**

- [Microsoft Graph 错误响应信息](https://docs.microsoft.com/graph/errors)
- [Microsoft Graph 已知问题](https://docs.microsoft.com/graph/known-issues)

**在哪里可以检查服务可用性和连接状态？**

可通过 Microsoft Graph 访问的基础服务的服务可用性和连接性可能会影响 Microsoft Graph 的总体可用性和性能。

- 对于 Azure Active Directory 服务运行状况，请检查 Azure 状态页中列出的安全 **+** [标识服务的状态](https://azure.microsoft.com/status/)。
- 对于参与 Microsoft Graph 的 Office 服务，请检查 Office 服务运行状况仪表板中列出的服务 [的状态](https://portal.office.com/adminportal/home#/servicehealth)。

Microsoft Graph 授权错误可能是多个不同问题的结果，大多数问题会产生 401 或 403 错误。 例如，以下情况可能会导致授权错误：

- 不正确的[访问令牌获取流](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- 配置不当的[权限范围](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- 缺乏[许可](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

**_对 Azure Active Directory 身份验证库 (ADAL) 和 Azure AD Graph API (AAD Graph) 的支持终止_* _

_*自 2020 年 6 月 30 日起，我们将不再向 ADAL 和 Azure AD Graph 添加任何新功能。 我们将继续提供技术支持和安全更新，但不再提供功能更新。

**从 2022** 年 6 月 30 日开始，我们将停止支持 ADAL 和 Azure AD Graph，并且将不再提供技术支持或安全更新。

在现有的操作系统版本上使用 ADAL 的应用在此时间之后将继续工作，但将不会获得 *任何技术支持或安全更新*。

在此时间之后，使用 Azure AD Graph 的应用可能不再收到来自 Azure AD Graph 终结点的响应。

**ADAL 迁移**

我们建议更新到具有最新功能和安全更新的 [Microsoft 身份验证库 (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)。

如果你使用的是 Microsoft 应用，请了解 Microsoft 正在将应用程序迁移到 MSAL（在支持终止截止时间之前）以确保他们将受益于 MSAL 正在进行的安全和功能改进。

1. [请阅读 ADAL 常见问题解答](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [了解如何在不同平台上迁移应用](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. 如果你需要帮助了解哪些应用使用 ADAL，我们建议你查看所有应用的源代码，如果适用，请联系任何 ISV 或应用提供商。 Microsoft 支持部门也可提供租户内所有非 Microsoft ADAL 应用的列表。

**AAD Graph 迁移**

对于使用 Azure AD Graph 的应用程序，请按照我们的指南将[Azure AD Graph 应用迁移到 Microsoft Graph。](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [我们的迁移清单提供了入门起点](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。
2. 你的 Azure 应用注册门户显示了哪些应用正在使用 AAD Graph。 我们建议查看应用的全部源代码，并且如果适用，请联系任何 ISV 或应用提供商。 Microsoft 支持还可以提供租户中所有 AAD Graph 使用情况的列表。
3. 若要使你的应用可访问 Microsoft Graph 中的数据，用户或管理员必须通过同意过程向其授予正确的权限。 [Microsoft Graph 权限参考](https://docs.microsoft.com/graph/permissions-reference)列出了与每组主要 Microsoft Graph API 关联的权限。 它还提供有关如何使用权限的指导。
