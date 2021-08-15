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
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013450"
---
# <a name="issues-developing-applications-with-apis"></a>使用 API 开发应用程序时的问题

若要开始使用 Azure Active Directory Graph API，请参阅[Azure AD Graph API 快速](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro)入门指南，或查看交互式[Azure AD Graph API 参考文档](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)。

**停止支持 ADAL Azure Active Directory ADAL (和 Azure AD) API Graph AAD (AAD Graph)**

**从 2020** 年 6 月 30 日开始，我们将不再将任何新功能添加到 ADAL 和 Azure AD Graph。 我们将继续提供技术支持和安全更新，但不再提供功能更新。

**从 2022** 年 6 月 30 日开始，我们将停止对 ADAL 和 Azure AD Graph将不再提供技术支持或安全更新。

此时间之后，在现有 OS 版本上使用 ADAL 的应用将继续工作，但将不会获得任何技术支持或安全更新。

此后，使用 Azure AD Graph 的应用可能不再接收来自 Azure AD Graph 端点的响应。

**ADAL 迁移**

我们建议更新到具有最新功能和安全更新的 [Microsoft 身份验证库 (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)。

如果你使用的是 Microsoft 应用，请了解 Microsoft 正在将应用程序迁移到 MSAL，直到停止提供支持的截止时间，确保他们将受益于 MSAL 正在进行的安全和功能改进。

1. [请阅读 ADAL 常见问题解答](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)。
1. [了解如何在不同平台上迁移应用](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)。
1. 如果你需要了解哪些应用使用 ADAL 的帮助，我们建议你查看所有应用的源代码，如果适用，请联系任何 ISV 或应用提供商。 Microsoft 支持部门也可提供租户内所有非 Microsoft ADAL 应用的列表。

**AAD Graph 迁移**

对于使用 Azure AD Graph，请按照我们的指南将[Azure AD Graph应用迁移到 Microsoft Graph。](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [我们的迁移清单提供了入门起点](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。 
1. 你的 Azure 应用注册门户显示了哪些应用正在使用 AAD Graph。 我们建议查看应用的全部源代码，并且如果适用，请联系任何 ISV 或应用提供商。 Microsoft 支持还可以提供租户中所有 AAD Graph列表。
1. 若要使你的应用可访问 Microsoft Graph 中的数据，用户或管理员必须通过同意过程向其授予正确的权限。 [Microsoft Graph权限](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true)参考列出了与每个主要 Microsoft 应用程序 API 集Graph的权限。 它还提供有关如何使用权限的指导。
