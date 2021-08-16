---
title: 将无缝 SSO 与本地应用集成的问题
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
ms.openlocfilehash: 6b295f3272ba074eac3afb66f3156af7ea4065a1398a215bcb3cde5da74b198a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028282"
---
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a>将无缝 SSO 与本地应用集成的问题

若要解决将无缝 SSO 与本地应用程序集成的问题，请执行下列操作：

**建议的步骤**

1. 若要通过应用程序 **代理** 为单一登录配置本地应用程序，请参阅使用应用程序代理的单一登录 [的密码保管](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)。
1. **应用程序代理问题** 疑难解答 ：我们建议你先查看疑难解答流，调试应用程序 [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)代理连接器问题，以确定应用程序代理连接器是否配置正确。 如果你仍然无法连接到应用，请按照[调试应用程序代理应用问题](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)中的步骤进行故障排除。 可以通过 [使用下列浏览器](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) 调试工具识别 CORS 问题：
    1. 启动浏览器并浏览 web 应用。
    1. 按下 **F12** 调出调试控制台。
    1. 尝试重现事务，并查看控制台消息。 若是 CORS 冲突问题，会出现关于来源的控制台错误。
    1. 某些 CORS 问题无法解决，例如，当应用重定向到 login.microsoftonline.com 进行身份验证时，访问令牌将过期。 然后 CORS 调用将失败。 此情况的解决方法之一是延长访问令牌的生命周期，来防止其在用户会话期间过期。 有关如何操作的详细信息，请参阅[Microsoft 标识平台中可配置的令牌生命周期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。

**推荐文档**

- [如何配置应用程序代理应用程序的单一登录](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [使用应用程序代理本地应用程序的 SAML 单一登录](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [了解并解决Azure Active Directory代理 CORS 问题](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [应用程序代理 Kerberos 约束委派配置故障排除](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)