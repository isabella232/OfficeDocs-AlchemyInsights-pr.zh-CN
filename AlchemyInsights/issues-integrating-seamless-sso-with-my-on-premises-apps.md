---
title: 将无缝 SSO 与本地应用集成时的问题
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "7798"
ms.openlocfilehash: 785d7f842031c1056ec6868376f253439919a3ab
ms.sourcegitcommit: 227a949a6ae49cc52c7fdcef2f9fd202c746169d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/13/2021
ms.locfileid: "49848768"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>将无缝 SSO 与本地应用集成时的问题

若要解决将无缝 SSO 与本地应用程序集成的问题，请执行下列操作：

**建议的步骤**

1. 若要通过应用程序 **代理** 为单一登录配置本地应用程序，请参阅"使用应用程序代理单一登录的密码保管 ["。](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)
1. **应用程序代理问题疑难解答**：我们建议您首先查看疑难解答流，调试应用程序代理 [连接器](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)问题，以确定应用程序代理连接器是否配置正确。 如果连接到应用程序时仍遇到问题，请按照调试应用程序代理应用程序问题中的疑难 [解答步骤操作](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)。 可以通过 [使用下列浏览器](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) 调试工具识别 CORS 问题：
    1. 启动浏览器并浏览到 Web 应用。
    1. 按 **F12** 打开调试控制台。
    1. 尝试重现事务，并查看控制台消息。 CORS 冲突会产生有关源的控制台错误。
    1. 某些 CORS 问题无法解决，例如当你的应用重定向到login.microsoftonline.com进行身份验证时，访问令牌过期。 然后 CORS 调用将失败。 此方案的解决方法是延长访问令牌的生存期，以防止它在用户会话期间过期。 若要详细了解如何这样做，请参阅 Microsoft 标识平台中的可配置 [令牌生存期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。

**推荐文档**

- [如何配置应用程序代理应用程序的单一登录](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [使用应用程序代理本地应用程序的 SAML 单一登录](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [了解并解决 Azure Active Directory 应用程序代理 CORS 问题](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [应用程序代理的 Kerberos 约束委派配置疑难解答](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)