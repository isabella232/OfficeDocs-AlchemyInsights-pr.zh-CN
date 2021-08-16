---
title: 开发应用程序的问题
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
- "7754"
- "9004342"
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013414"
---
# <a name="issues-developing-applications"></a>开发应用程序的问题

若要在构建 Azure Active Directory (AD) 应用时解决最常见问题，请参阅下列文章：

- [我仅在使用 Chrome 浏览器登录应用程序时遇到问题](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [我不知道如何更改我的应用程序令牌生存期默认值](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [我不清楚应用程序许可的工作方式](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [我不知道如何向我的应用程序授予权限](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [我不了解委派和应用程序权限的区别](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***对 Azure Active Directory 身份验证库 (ADAL) 和 Azure AD Graph API (AAD Graph) 的支持终止***

- 自 2020 年 6 月 30 日起，我们将不再向 Azure Active Directory 身份验证库 (ADAL) 和 Azure AD Graph API (AAD Graph) 添加任何新功能。 我们将继续提供技术支持和安全更新，但不再提供功能更新。

- 自 2022 年 6 月 30 日起，我们将终止对 ADAL 和 AAD Graph 的支持，并且将不再提供技术支持或安全更新。 此条件的含义如下所述：

    - 此时间之后，在现有 OS 版本上使用 ADAL 的应用将继续工作，但将不会获得任何技术支持或安全更新。

    - 此时间之后，使用 AAD Graph 的应用将不再接收来自 AAD Graph 终结点的响应。

**ADAL 迁移**

如果正在使用 Microsoft 应用，我们建议更新到具有最新功能和安全更新的 Microsoft 身份验证库 (MSAL)。 此建议是在 Microsoft 启动在支持结束截止日期之前将其应用迁移到 MSAL 的过程背景下提出的。 

Microsoft 将应用迁移到 MSAL 可确保应用从 MSAL 持续的安全与功能改进中受益。

1. [请阅读 ADAL 常见问题解答](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [了解如何在不同平台上迁移应用](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. 如果在了解哪些应用使用 ADAL 方面需要帮助，我们建议查看应用的全部源代码，如果适用，还请联系任何独立软件供应商 (ISV) 或应用提供商。 Microsoft 支持部门也可提供租户内所有非 Microsoft ADAL 应用的列表。

**AAD Graph 迁移**

对于使用 AAD Graph 的应用程序，请遵循我们关于迁移 AAD Graph 应用到 Microsoft Graph 的指南：

1. [我们的迁移清单提供了入门起点](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。 
2. 你的 Azure 应用注册门户显示了哪些应用正在使用 AAD Graph。 我们建议查看应用的全部源代码，并且如果适用，请联系任何独立软件销售商 (ISV) 或应用提供商。 Microsoft 支持部门也可提供租户内 AAD Graph 使用情况的信息。







