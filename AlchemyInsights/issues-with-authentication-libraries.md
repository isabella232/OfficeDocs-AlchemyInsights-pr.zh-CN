---
title: 身份验证库问题
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
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2021
ms.locfileid: "50037210"
---
# <a name="issues-with-authentication-libraries"></a>身份验证库问题

1. [Microsoft 标识平台身份验证库](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) 列出了 Microsoft 支持的兼容客户端和中间件库。
2. Microsoft 身份验证库 (MSAL) [支持多个](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) 身份验证流，以用于不同的应用程序方案。
3. 若要进行身份验证和获取令牌，您可以在代码中初始化新的公共或机密客户端应用程序。 在 MICROSOFT 身份验证库或 MSAL (中初始化客户端应用时，可以设置) 。 若要了解详细信息，请参阅 [应用程序配置选项](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)。

**停止支持 Azure Active Directory 身份验证库 (ADAL) 和 Azure AD Graph API (AAD Graph)**

**从 2020** 年 6 月 30 日开始，我们将不再向 ADAL 和 Azure AD Graph 添加任何新功能。 我们将继续提供技术支持和安全更新，但不再提供功能更新。

**从 2022** 年 6 月 30 日开始，我们将停止对 ADAL 和 Azure AD Graph 的支持，并且将不再提供技术支持或安全更新。

在现有的操作系统版本上使用 ADAL 的应用在此时间之后将继续工作，但将不会获得 *任何技术支持或安全更新*。

在此时间之后使用 Azure AD Graph 的应用可能不再收到来自 Azure AD Graph 终结点的响应。

**ADAL 迁移**

我们建议更新到具有最新功能和安全更新的 [Microsoft 身份验证库 (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)。

如果你使用的是 Microsoft 应用，请知道 Microsoft 正在将应用程序迁移到 MSAL，直到支持期限结束，确保他们将受益于 MSAL 正在进行的安全和功能改进。

有关详细信息，请参阅：

1. [请阅读 ADAL 常见问题解答](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [了解如何在不同平台上迁移应用](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. 如果你需要了解哪些应用使用 ADAL 的帮助，我们建议你查看所有应用的源代码，如果适用，请联系任何 ISV 或应用提供商。 Microsoft 支持部门也可提供租户内所有非 Microsoft ADAL 应用的列表。

**AAD Graph 迁移**

对于使用 Azure AD Graph 的应用程序，请按照我们的指南将[Azure AD Graph 应用迁移到 Microsoft Graph。](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [我们的迁移清单提供了一个入门点。](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. 你的 Azure 应用注册门户显示了哪些应用正在使用 AAD Graph。 我们建议查看应用的全部源代码，并且如果适用，请联系任何 ISV 或应用提供商。 Microsoft 支持还可以提供租户中所有 AAD Graph 使用情况的列表。
3. 若要使你的应用可访问 Microsoft Graph 中的数据，用户或管理员必须通过同意过程向其授予正确的权限。 [Microsoft Graph 权限参考](https://docs.microsoft.com/graph/permissions-reference)列出了与每组主要 Microsoft Graph API 关联的权限。 它还提供有关如何使用权限的指导。
