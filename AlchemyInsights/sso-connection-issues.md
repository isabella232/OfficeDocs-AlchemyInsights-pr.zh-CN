---
title: SSO 连接问题
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
- "9004357"
- "7810"
ms.openlocfilehash: 8fb93bc40c6cd5a7c0e3d259fe3be8d1bab3187dd5aa023eb49977555fd930de
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084336"
---
# <a name="sso-connection-issues"></a>SSO 连接问题

1. 按照 [快速入门：配置应用的属性](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure)指南来配置你的应用。
2. 根据你选择的应用程序和 [单一登录](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) 选项，请按照下面的相应指南操作：
    - 若要 **为基于****SAML** 的单一登录配置本地应用程序，请参阅 [SAML single-sign-on for on-premises applications with Application Proxy。](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
    - 若要为 **基于密码** 的单一登录配置云 **应用程序**，请参阅  [配置密码单一登录](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)。
    - 若要通过应用程序 **代理** 为单一登录配置本地应用程序，请参阅使用应用程序代理的单一登录 [的密码保管](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)。
3. **应用程序代理问题** 疑难解答 ：我们建议你先查看疑难解答流，调试 [](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)应用程序代理连接器问题，以确定应用程序代理连接器是否配置正确。 如果连接到应用程序时仍有问题，请按照调试应用程序代理应用程序问题中的疑难 [解答流程操作](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)。 可以使用 [浏览器调试工具识别 CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) 问题：
    - 启动浏览器并浏览 web 应用。
    - 按下 **F12** 调出调试控制台。
    - 尝试重现事务，并查看控制台消息。 若是 CORS 冲突问题，会出现关于来源的控制台错误。
    - 某些 CORS 问题无法解决，例如，当应用重定向到 login.microsoft.com 进行身份验证时，访问令牌将过期。 然后 CORS 调用将失败。 此情况的解决方法之一是延长访问令牌的生命周期，来防止其在用户会话期间过期。 有关如何操作的详细信息，请参阅[Microsoft 标识平台中可配置的令牌生命周期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。
4. **对基于 SAML 的单** 一登录进行故障排除 ：我们建议检查登录到基于 [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)的单一登录配置的应用时遇到的问题，以查找你最有可能遇到的问题的解决方案。
5. **基于密码的单** 一登录疑难解答 ：我们建议在 [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)中检查基于密码的单一登录疑难解答，以查找最可能遇到的问题的解决方案。
6. 有关使用 VPN 时的连接问题，请参阅如何使用通过 VPN ([SSO](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)) 单一Wi-Fi登录。
