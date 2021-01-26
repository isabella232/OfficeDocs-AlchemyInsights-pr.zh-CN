---
title: 查询 Microsoft Graph API
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950665"
---
# <a name="querying-the-microsoft-graph-api"></a>查询 Microsoft Graph API

本主题还适用于仍在使用 Azure AD Graph API 的开发人员。 但是， **强烈建议** 将 Microsoft Graph 用于所有目录、标识和访问管理方案。

**身份验证或授权问题**

- 如果你的应用无法获取令牌来调用 Microsoft Graph，请选择"获取访问令牌 **(身份验证)** Microsoft Graph"类别以获取有关本主题的更具体的帮助和支持。
- 如果你的应用在调用 Microsoft Graph 时收到 **401 或 403** 授权错误，请选择"获取访问被拒绝错误 **(授权)** Microsoft Graph API"类别，获取有关本主题的更具体的帮助和支持。

**我想要使用 Microsoft Graph，但不确定从何处开始**

若要了解有关 Microsoft Graph 的更多信息，请参阅：

- [Microsoft Graph 概述](https://docs.microsoft.com/graph/overview)
- [Microsoft Graph 中的标识和访问管理概述](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [开始构建 Microsoft Graph 应用](https://docs.microsoft.com/graph/)
- **Microsoft Graph 资源管理器** - 在租户或演示租户中测试 Microsoft Graph API

**我想要使用 Microsoft Graph，但它是否支持所需的 v1.0 目录 API？**

Microsoft Graph 是推荐的目录、标识和访问管理的 API。 但是，Azure AD Graph 和 Microsoft Graph 中可能存在一些差异。 请查看以下文章，其中重点介绍了最新的差异，以帮助你做出选择：

- [Azure AD Graph 和 Microsoft Graph 之间的资源类型差异](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD Graph 和 Microsoft Graph 之间的属性差异](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD 和 Microsoft Graph 之间的方法差异](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**当我查询 *用户对象* 时，其许多属性都缺失**

`GET https://graph.microsoft.com/v1.0/users` 仅返回 11 个属性，因为 Microsoft Graph 自动选择要返回的默认 *用户* 属性集。 如果需要其他用户 *属性，* 请使用$select来选取应用程序所需的属性。 首先在 **Microsoft Graph 资源管理器中试用** 。

**一些用户属性值 *为 null，* 即使我们知道它们已设置**

最可能的解释是应用程序已被授予 *User.ReadBasic.All* 权限。 这允许应用程序读取一组有限的用户属性，将所有其他属性返回为 null，即使之前已设置这些属性。 请尝试改为授予应用程序 *User.Read.All* 权限。

有关详细信息，请参阅 [Microsoft Graph 用户权限](https://docs.microsoft.com/graph/permissions-reference#user-permissions)。

**我在使用 OData 查询参数筛选请求中数据时遇到问题**

虽然 Microsoft Graph 支持各种 OData 查询参数，但从 Microsoft Graph 中的 *directoryObject*) 继承的目录服务 (资源并不完全支持这些参数。 在 Microsoft Graph 中，Azure AD Graph 中的大多数限制仍然存在：

1. **不支持**：$count、$search，$filter null 值 *或不**为 null* 值时返回
2. **不支持：$filter** 某些属性 (查看有关哪些属性可筛选的资源) 
3. **不支持**：同时分页、筛选和排序
4. **不支持：** 对关系进行筛选。 例如，查找英国工程组的所有成员。
5. **部分支持**：$orderby *displayName* 和 userPrincipalName (displayName 和 userPrincipalName *) 组*
6. **部分支持**：$filter (仅支持 *eq* *、startswith**或*，*以及*，并限制任何 *)* 支持，$expand (展开单个对象的关系将返回所有关系，但扩展对象的关系集合是有限的) 

有关详细信息，请参阅使用 [查询参数自定义响应](https://docs.microsoft.com/graph/query-parameters)。

**我调用的 API 不起作用 - 在哪里可以执行更多测试？**

**Microsoft Graph 资源管理器**- 在租户或演示租户中测试 Microsoft Graph API，并查看 Microsoft Graph 资源管理器中的示例查询。 

**当我查询数据时，似乎我重新设置了不完整的数据**

如果要像用户 (查询集合) ，Microsoft Graph将使用服务器端页面限制，以便始终返回具有默认页面大小的结果。 你的应用应始终希望浏览从服务返回的集合。

有关详细信息，请参阅：

- [Microsoft Graph 最佳实践](https://docs.microsoft.com/graph/best-practices-concept)
- [在应用中对 Microsoft Graph 数据进行分页](https://docs.microsoft.com/graph/paging)

**我的应用过慢，并且也受到限制。我可以进行哪些改进？**

根据你的方案，有多种不同的选项可供选择，使应用程序更具有性能;在某些情况下，当您对应用程序进行过多调用时，服务 (很容易受到) 。

有关详细信息，请参阅：

- [Microsoft Graph 最佳实践](https://docs.microsoft.com/graph/best-practices-concept)
- [批处理请求](https://docs.microsoft.com/graph/json-batching)
- [通过 delta 查询跟踪更改](https://docs.microsoft.com/graph/delta-query-overview)
- [通过 Webhook 获取更改通知](https://docs.microsoft.com/graph/webhooks)
- [限制指南](https://docs.microsoft.com/graph/throttling)

**在哪里可以找到有关错误和已知问题的详细信息？**

- [Microsoft Graph 错误响应信息](https://docs.microsoft.com/graph/errors)
- [Microsoft Graph 已知问题](https://docs.microsoft.com/graph/known-issues)

**在哪里可以检查服务可用性和连接状态？**

可通过 Microsoft Graph 访问的基础服务的服务可用性和连接可能会影响 Microsoft Graph 的总体可用性和性能。

- 对于 Azure Active Directory 服务运行状况，请检查 Azure 状态页中列出的安全 **+** [标识服务的状态](https://azure.microsoft.com/status/)。
- 对于参与 Microsoft Graph 的 Office 服务，请检查 Office 服务运行状况仪表板中列出的 [服务的状态](https://portal.office.com/adminportal/home#/servicehealth)。
