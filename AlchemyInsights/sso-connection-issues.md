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
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2021
ms.locfileid: "49918135"
---
# <a name="sso-connection-issues"></a><span data-ttu-id="87638-102">SSO 连接问题</span><span class="sxs-lookup"><span data-stu-id="87638-102">SSO Connection Issues</span></span>

1. <span data-ttu-id="87638-103">按照 [快速入门：配置应用的属性](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure)指南来配置你的应用。</span><span class="sxs-lookup"><span data-stu-id="87638-103">Follow the [Quickstart: Configure properties for an application](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) guide to configure your application.</span></span>
2. <span data-ttu-id="87638-104">根据你选择的应用程序和 [单一登录](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) 选项，请按照下面的相应指南操作：</span><span class="sxs-lookup"><span data-stu-id="87638-104">Depending on the application and [Single sign-on option](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) you chose, follow the appropriate guidance below:</span></span>
    - <span data-ttu-id="87638-105">若要 **为基于\*\*\*\*SAML** 的单一登录配置本地应用程序，请参阅使用应用程序代理本地应用程序的 [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)单一登录。</span><span class="sxs-lookup"><span data-stu-id="87638-105">To configure an **on-premises application** for **SAML-based single sign-on**, see [SAML single-sign-on for on-premises applications with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).</span></span>
    - <span data-ttu-id="87638-106">若要为 **基于密码** 的单一登录配置云 **应用程序**，请参阅 ["配置密码单一登录"。](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)</span><span class="sxs-lookup"><span data-stu-id="87638-106">To configure a **cloud application** for **password-based single sign-on**, see  [Configure password single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications).</span></span>
    - <span data-ttu-id="87638-107">若要通过应用程序 **代理** 为单一登录配置本地应用程序，请参阅使用应用程序代理进行单一登录的密码 [保管](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)。</span><span class="sxs-lookup"><span data-stu-id="87638-107">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
3. <span data-ttu-id="87638-108">**应用程序代理问题疑难解答**：我们建议您首先查看疑难解答流，调试应用程序代理 [连接器](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)问题，以确定应用程序代理连接器是否配置正确。</span><span class="sxs-lookup"><span data-stu-id="87638-108">**Troubleshooting Application Proxy issues**: we recommend you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="87638-109">如果连接到应用程序时仍遇到问题，请按照调试应用程序代理应用程序问题中的疑难 [解答流操作](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)。</span><span class="sxs-lookup"><span data-stu-id="87638-109">If you are still having trouble connecting to the application, follow the troubleshooting flow in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="87638-110">可以使用 [浏览器调试工具识别 CORS](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) 问题：</span><span class="sxs-lookup"><span data-stu-id="87638-110">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using browser debug tools:</span></span>
    - <span data-ttu-id="87638-111">启动浏览器并浏览 web 应用。</span><span class="sxs-lookup"><span data-stu-id="87638-111">Launch the browser and browse to the web app.</span></span>
    - <span data-ttu-id="87638-112">按下 **F12** 调出调试控制台。</span><span class="sxs-lookup"><span data-stu-id="87638-112">Press **F12** to bring up the debug console.</span></span>
    - <span data-ttu-id="87638-113">尝试重现事务，并查看控制台消息。</span><span class="sxs-lookup"><span data-stu-id="87638-113">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="87638-114">若是 CORS 冲突问题，会出现关于来源的控制台错误。</span><span class="sxs-lookup"><span data-stu-id="87638-114">A CORS violation produces a console error about origin.</span></span>
    - <span data-ttu-id="87638-115">某些 CORS 问题无法解决，例如当应用重定向到login.microsoft.com进行身份验证时，访问令牌过期。</span><span class="sxs-lookup"><span data-stu-id="87638-115">Some CORS issues can't be resolved, such as when your app redirects to login.microsoft.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="87638-116">然后 CORS 调用将失败。</span><span class="sxs-lookup"><span data-stu-id="87638-116">The CORS call then fails.</span></span> <span data-ttu-id="87638-117">此情况的解决方法之一是延长访问令牌的生命周期，来防止其在用户会话期间过期。</span><span class="sxs-lookup"><span data-stu-id="87638-117">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="87638-118">有关如何操作的详细信息，请参阅[Microsoft 标识平台中可配置的令牌生命周期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。</span><span class="sxs-lookup"><span data-stu-id="87638-118">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>
4. <span data-ttu-id="87638-119">**基于 SAML** 的单一登录疑难解答：我们建议检查登录到基于 [SAML](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery)的单一登录配置的应用时遇到的问题，以查找你最有可能遇到的问题的解决方案。</span><span class="sxs-lookup"><span data-stu-id="87638-119">**Troubleshooting SAML-based single sign-on**: we recommend checking [Problems signing in to SAML-based single sign-on configured apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery), to find the solutions to the issues you are most likely to encounter.</span></span>
5. <span data-ttu-id="87638-120">**基于密码的单** 一登录疑难解答：我们建议在 [Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)中检查基于密码的单一登录疑难解答，以查找最可能遇到的问题的解决方案。</span><span class="sxs-lookup"><span data-stu-id="87638-120">**Troubleshooting password-based single sign-on**: we recommend checking [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), to find the solutions to the issues you are most likely to encounter.</span></span>
6. <span data-ttu-id="87638-121">有关使用 VPN 时的连接问题，请参阅如何通过 VPN ([SSO](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections)) 单一登录Wi-Fi连接。</span><span class="sxs-lookup"><span data-stu-id="87638-121">For connection issues while using a VPN, see [How to use single sign on (SSO) over VPN and Wi-Fi connections](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).</span></span>