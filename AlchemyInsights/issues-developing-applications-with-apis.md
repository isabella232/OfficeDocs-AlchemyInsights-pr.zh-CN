---
title: 使用 API 开发应用程序时的问题
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
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951874"
---
# <a name="issues-developing-applications-with-apis"></a>使用 API 开发应用程序时的问题

若要开始使用 Azure Active Directory Graph API，请参阅 [Azure AD Graph API 快速入门指南](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ，或查看 [交互式 Azure AD Graph API 参考文档](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)。

**停止支持 Azure Active Directory 身份验证库 (ADAL) 和 Azure AD Graph API (AAD Graph)**

**从 2020** 年 6 月 30 日开始，我们将不再向 ADAL 和 Azure AD Graph 添加任何新功能。 我们将继续提供技术支持和安全更新，但将不再提供功能更新。

**从 2022** 年 6 月 30 日开始，我们将停止对 ADAL 和 Azure AD Graph 的支持，并且将不再提供技术支持或安全更新。

在现有的操作系统版本上使用 ADAL 的应用在此时间之后将继续工作，但将不会获得任何技术支持或安全更新。

在此时间之后使用 Azure AD Graph 的应用可能不再收到来自 Azure AD Graph 终结点的响应。

**ADAL 迁移**

我们建议更新到 [具有最新功能和安全更新 (MSAL) ](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)Microsoft 身份验证库。

如果你使用的是 Microsoft 应用，请知道 Microsoft 正在将应用程序迁移到 MSAL（在支持终止截止时间之前）以确保他们将受益于 MSAL 正在进行的安全和功能改进。

1. [阅读 ADAL 常见问题解答](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)。
1. [了解如何基于每个平台迁移应用](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)。
1. 如果你需要了解哪些应用使用 ADAL 的帮助，我们建议你查看所有应用的源代码，如果适用，请联系任何 ISV 或应用提供商。 Microsoft 支持还可以提供租户中所有非 Microsoft ADAL 应用的列表。

**AAD Graph 迁移**

对于使用 Azure AD Graph 的应用程序，请按照我们的指南将[Azure AD Graph 应用迁移到 Microsoft Graph。](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [我们的迁移清单提供了一个入门点](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。 
1. Azure 应用注册门户显示哪些应用程序正在使用 AAD Graph。 我们建议你查看所有应用的源代码，如果适用，请联系任何 ISV 或应用提供商。 Microsoft 支持还可以提供租户中所有 AAD Graph 使用情况的列表。
1. 若要使你的应用可访问 Microsoft Graph 中的数据，用户或管理员必须通过同意过程向其授予正确的权限。 [Microsoft Graph 权限参考](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true)列出了与每组主要 Microsoft Graph API 关联的权限。 它还提供有关如何使用权限的指导。
