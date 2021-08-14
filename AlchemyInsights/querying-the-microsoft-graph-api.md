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
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923229"
---
# <a name="querying-the-microsoft-graph-api"></a>查询 Microsoft Graph API

本主题还适用于仍在使用 Azure AD Graph API 的开发人员。 但是，**强烈建议** 将 Microsoft Graph用于所有目录、标识和访问管理方案。

**身份验证或授权问题**

- 如果你的应用无法获取调用 Microsoft Graph 的令牌，请选择"获取访问令牌 **的问题 (身份验证)** Microsoft Graph"类别，获取有关本主题的更具体的帮助和支持。
- 如果你的应用在调用 Microsoft Graph 时收到 **401 或 403** 授权错误，请选择"获取访问被拒绝错误 **(授权)** Microsoft Graph API"类别，获取有关本主题的更具体的帮助和支持。

**我想要使用 Microsoft Graph，但不确定从何处开始**

若要了解有关 Microsoft Graph，请参阅：

- [Microsoft Graph 概述](https://docs.microsoft.com/graph/overview)
- [Microsoft 服务中的标识和访问管理Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [开始构建 Microsoft Graph应用](https://docs.microsoft.com/graph/)
- **Microsoft Graph资源管理器**- Graph租户或演示租户中测试 Microsoft api

**我想要使用 Microsoft Graph，但它是否支持所需的 v1.0 目录 API？**

Microsoft Graph 是推荐的用于目录、标识和访问管理的 API。 但是，Azure AD 应用程序与 Microsoft Graph 之间仍有一些Graph。 查看以下文章，这些文章重点介绍了可帮助你做出选择的最最新差异：

- [Azure AD 应用程序与 Microsoft Graph 之间的资源类型Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD Graph 和 Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD 和 Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**当我查询 *用户对象* 时，它的许多属性都缺失**

`GET https://graph.microsoft.com/v1.0/users`仅返回 11 个属性，因为 Microsoft Graph自动选择要返回的默认 *用户* 属性集。 如果需要其他用户 *属性，* 请使用 $select来选取应用程序所需的属性。 首先在 Microsoft Graph **资源管理器中** 试用。

**一些用户属性值为 *null，* 即使你知道它们已设置**

最可能的解释是应用程序已被授予 *User.ReadBasic.All* 权限。 这允许应用程序读取一组有限的用户属性，以 null 返回所有其他属性，即使之前已设置这些属性。 尝试改为授予应用程序 *User.Read.All* 权限。

有关详细信息，请参阅[Microsoft Graph用户权限](https://docs.microsoft.com/graph/permissions-reference#user-permissions)。

**我在使用 OData 查询参数筛选请求中数据时遇到问题**

虽然 Microsoft Graph 支持多种 OData 查询参数，但许多这些参数不受从 Microsoft Graph 中的 *directoryObject*) 继承的目录服务 (资源完全支持。 Azure AD 中的相同限制在大部分Graph在 Microsoft Graph：

1. **不支持**：$count、$search 和 $filter *null 值* 或不为 *null* 值
2. **不支持：$filter** 某些属性 (有关哪些属性可筛选的资源主题) 
3. **不支持**：同时分页、筛选和排序
4. **不支持 ：** 对关系进行筛选。 例如 - 查找英国工程组的所有成员。
5. **部分支持**：$orderby *displayName* 和 userPrincipalName (displayName 和 userPrincipalName 仅 *) 组*
6. **部分** 支持：$filter (仅支持 *eq、startswith、or* 和 *，并* 限制任何 *)* 支持，$expand (展开单个对象的关系将返回所有关系，但扩展对象的关系集合)  

有关详细信息，请参阅使用 [查询参数自定义响应](https://docs.microsoft.com/graph/query-parameters)。

**我调用的 API 不起作用 - 在哪里可以执行更多测试？**

**Microsoft Graph资源管理器**- 在租户或演示租户中测试 Microsoft Graph API，并查看 Microsoft Graph资源管理器中的示例查询。

**当我查询数据时，似乎我重新设置了不完整的数据**

如果您要像用户 (查询集合) ，Microsoft Graph会使用服务器端页面限制，因此始终使用默认页面大小返回结果。 你的应用应始终希望分页查看从服务返回的集合。

有关详细信息，请参阅：

- [Microsoft Graph最佳实践](https://docs.microsoft.com/graph/best-practices-concept)
- [在应用中对 Microsoft Graph 数据进行分页](https://docs.microsoft.com/graph/paging)

**我的应用过慢，并且也受到限制。我可以进行哪些改进？**

根据你的方案，可以使用各种不同的选项来使应用程序性能提高，并且在某些情况下，当您在) 中执行过多调用时，服务 (很容易被限制。

有关详细信息，请参阅：

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
