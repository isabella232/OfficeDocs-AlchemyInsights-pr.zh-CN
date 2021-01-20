---
title: SSO 配置问题
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7760"
- "9004346"
ms.openlocfilehash: 5ab56ec1eda10ea059e600e8933ce85bb143b76e
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886785"
---
# <a name="sso-configuration-issues"></a>SSO 配置问题

1. 按照 [快速入门：配置应用的属性](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure)指南来配置你的应用。
2. 取决于应用和你选择的[单一登陆选项](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options)，按照下列的指南进行合适的操作：a. 要配置 **基于 SAML 的单一登陆 (SSO)** 的 **本地应用**，请参阅[使用应用程序代理的本地应用 SAML 单一登陆](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)。
    b. 要配置 **基于密码的 SSO** 的 **云应用**，请参阅[配置密码单一登陆](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)。
    c. 要配置 **使用应用代理的 SSO** 的 **本地应用**，请参阅[使用应用程序代理的单一登陆密码路径](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)。
3. **应用程序代理问题故障排除**：我们建议首先查看故障排除工作流 - [调试应用程序代理连接器问题](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors) - 来判断应用程序代理连接器是否正确配置。 如果你仍然无法连接到应用，请按照[调试应用程序代理应用问题](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)中的步骤进行故障排除。 你可以通过执行以下浏览器调试步骤来[确定 CORS 问题](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues)。 启动浏览器并浏览 web 应用。
    b. 按下 **F12** 调出调试控制台。
    c. 尝试重现交易并查看控制台消息。 若是 CORS 冲突问题，会出现关于来源的控制台错误。
    d. 某些 CORS 问题无法解决，比如当应用重点向至 login.microsoftonline.com 进行验证时访问令牌过期。 由于访问令牌过期，CORS 调用失败。 此情况的解决方法之一是延长访问令牌的生命周期，来防止其在用户会话期间过期。 有关如何操作的详细信息，请参阅[Microsoft 标识平台中可配置的令牌生命周期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。
4. **基于 SAML 的 SSO 故障排除**：我们建议查看[登录到基于 SAML 的单一登陆配置应用相关问题](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)来查找你最有可能遇到的问题的解决方案。
5. **基于密码的 SSO 故障排除**：我们建议查看[在 Azure AD 中基于密码的单一登陆故障排除](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)来查找你最有可能遇到的问题的解决方案。
6. **我收到了配置错误**：排除配置错误的故障，我们建议查看下列文章：a. [登录到基于 SAML 的单一登陆配置应用的问题](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) b. [输入了证书，但是拓展无法提交它们](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso#credentials-are-filled-in-but-the-extension-does-not-submit-them) c. [输入并提交了证书，但是页面提示证书不正确](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) d. [用户登录后应用页面显示错误消息](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
7. **将无缝 SSO 和我的本地应用集成时遇到问题**：要故障排除有关 SSO 和本地应用集成的问题，我们建议阅读下列文章：a. [如何配置应用程序代理应用的单一登陆](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to) b. [使用应用程序代理进行本地应用 SAML 单一登陆](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps) c. [了解并解决 Azure Active Directory 应用程序代理 CORS 问题](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues) d. [应用程序代理 Kerberos 约束委派配置故障排除](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)
8. **我需要解决声明或延长令牌生命周期。我需要更改会话的长度**：如果是这样，我们建议阅读下列文章：a. [自定义发送到应用的 SAML 声明](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) b. [使用感知声明的应用](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) c. [Microsoft 标识平台中可配置令牌的生命周期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) d. [使用条件访问配置身份验证会话管理](https://docs.microsoft.com/azure/active-directory/conditional-access/howto-conditional-access-session-lifetime) e. [访问本地应用的 Cookie 设置](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-cookie-settings)
9. **我需要帮助管理我的用户和来宾用户 (B2B) 的访问权限**：有关管理用户和来宾用户访问权限的详细信息，我们建议阅读下列文章：a. [管理应用访问权限](https://docs.microsoft.com/azure/active-directory/manage-apps/what-is-access-management) b. [在 Azure Active Directory 中管理应用的用户分配](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) c. [为 B2B 协作配置 SaaS 应用](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) d. [授权 Azure AD 中的 B2B 用户访问本地应用的权限](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps) e. [使用 Azure AD B2B 协作将本地托管的合作伙伴账户权限授权给云资源](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)
10. **我想自定义我的应用**：有关自定义应用的详细信息，我们建议阅读下列文章：a. [使用 Azure AD 应用程序代理配置自定义域](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-domain) b. [为发布的应用设置自定义主页](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-custom-home-page) c. [通配符应用](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-wildcard)
11. **我在从 AD FS 迁移到 Azure 时遇到问题**：要故障排除在将应用从 AD FS 迁移到 Azure 时遇到的问题，我们建议阅读下列文章：a. [将应用的身份验证从 Active Directory 联合身份验证服务移动到 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/migrate-adfs-apps-to-azure) b. [有关迁移应用到 Azure Active Directory 的资源](https://docs.microsoft.com/azure/active-directory/manage-apps/migration-resources)

