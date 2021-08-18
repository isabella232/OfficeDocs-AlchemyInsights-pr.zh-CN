---
title: 配置和延长令牌生存期
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: ce100fcc2c62d62477f78e10b3cc9233fc2f5c5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329076"
---
# <a name="configure-and-extend-token-lifetimes"></a>配置和延长令牌生存期

您可以指定由 Microsoft 标识平台颁发的访问、SAML 或 ID 令牌的生存期。 可以为组织中的所有应用程序、多租户（多组织）应用程序或组织中的特定服务主体设置令牌生存期。 有关更多信息，请阅读[可配置令牌生存期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。

例如，阅读[如何配置令牌生存期的示例](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)。

要了解如何在 Azure Active Directory B2C (Azure AD B2C) 中配置令牌的生存期和兼容性，请参阅[在 Azure Active Directory B2C 中配置令牌](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow)。

文章[在 Azure Active Directory B2C 中配置会话行为](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow)描述了 Azure AD B2C 中使用的单一登录 (SSO) 方法，并帮助你在配置策略时选择最合适的 SSO 方法。

**令牌能用多久？有效期是多久？**

令牌生存期为 1 小时，会话生存期为 24 小时。 这意味着，如果 24 小时内没有任何请求，则需要在请求新令牌之前再次登录。

**注意**：2020 年 5 月 30 日之后，新租户将无法使用可配置令牌生存期策略来配置会话和刷新令牌。 弃用将在之后的几个月内发生，这意味着我们将停止执行现有会话并刷新令牌策略。 仍然可以在弃用之后配置访问令牌生存期。






