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
# <a name="issues-with-integrating-seamless-sso-with-my-on-premises-apps"></a><span data-ttu-id="3b7b7-102">将无缝 SSO 与本地应用集成时的问题</span><span class="sxs-lookup"><span data-stu-id="3b7b7-102">Issues with integrating Seamless SSO with my on-premises apps</span></span>

<span data-ttu-id="3b7b7-103">若要解决将无缝 SSO 与本地应用程序集成的问题，请执行下列操作：</span><span class="sxs-lookup"><span data-stu-id="3b7b7-103">To troubleshoot issues with integrating Seamless SSO with on-premises applications, do the following:</span></span>

<span data-ttu-id="3b7b7-104">**建议的步骤**</span><span class="sxs-lookup"><span data-stu-id="3b7b7-104">**Recommended steps**</span></span>

1. <span data-ttu-id="3b7b7-105">若要通过应用程序 **代理** 为单一登录配置本地应用程序，请参阅"使用应用程序代理单一登录的密码保管 ["。](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting)</span><span class="sxs-lookup"><span data-stu-id="3b7b7-105">To configure an **on-premises application** for **single sign-on through Application Proxy**, see [Password vaulting for single sign-on with Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).</span></span>
1. <span data-ttu-id="3b7b7-106">**应用程序代理问题疑难解答**：我们建议您首先查看疑难解答流，调试应用程序代理 [连接器](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors)问题，以确定应用程序代理连接器是否配置正确。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-106">**Troubleshooting Application Proxy issues**: we recommend that you start with reviewing the troubleshooting flow, [Debug Application Proxy Connector issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), to determine if Application Proxy connectors are configured correctly.</span></span> <span data-ttu-id="3b7b7-107">如果连接到应用程序时仍遇到问题，请按照调试应用程序代理应用程序问题中的疑难 [解答步骤操作](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps)。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-107">If you're still having trouble connecting to the application, follow the troubleshooting steps in [Debug Application Proxy application issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps).</span></span> <span data-ttu-id="3b7b7-108">可以通过 [使用下列浏览器](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) 调试工具识别 CORS 问题：</span><span class="sxs-lookup"><span data-stu-id="3b7b7-108">You can [identify CORS issues](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) by using the following browser debug tools:</span></span>
    1. <span data-ttu-id="3b7b7-109">启动浏览器并浏览到 Web 应用。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-109">Launch the browser and browse to the web app.</span></span>
    1. <span data-ttu-id="3b7b7-110">按 **F12** 打开调试控制台。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-110">Press **F12** to bring up the debug console.</span></span>
    1. <span data-ttu-id="3b7b7-111">尝试重现事务，并查看控制台消息。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-111">Try to reproduce the transaction, and review the console message.</span></span> <span data-ttu-id="3b7b7-112">CORS 冲突会产生有关源的控制台错误。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-112">A CORS violation produces a console error about origin.</span></span>
    1. <span data-ttu-id="3b7b7-113">某些 CORS 问题无法解决，例如当你的应用重定向到login.microsoftonline.com进行身份验证时，访问令牌过期。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-113">Some CORS issues can't be resolved, such as when your app redirects to login.microsoftonline.com to authenticate, and the access token expires.</span></span> <span data-ttu-id="3b7b7-114">然后 CORS 调用将失败。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-114">The CORS call then fails.</span></span> <span data-ttu-id="3b7b7-115">此方案的解决方法是延长访问令牌的生存期，以防止它在用户会话期间过期。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-115">A workaround for this scenario is to extend the lifetime of the access token, to prevent it from expiring during a user’s session.</span></span> <span data-ttu-id="3b7b7-116">若要详细了解如何这样做，请参阅 Microsoft 标识平台中的可配置 [令牌生存期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。</span><span class="sxs-lookup"><span data-stu-id="3b7b7-116">For more information about how to do this, see [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="3b7b7-117">**推荐文档**</span><span class="sxs-lookup"><span data-stu-id="3b7b7-117">**Recommended documents**</span></span>

- [<span data-ttu-id="3b7b7-118">如何配置应用程序代理应用程序的单一登录</span><span class="sxs-lookup"><span data-stu-id="3b7b7-118">How to configure single sign-on to an Application Proxy application</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-sso-how-to)
- [<span data-ttu-id="3b7b7-119">使用应用程序代理本地应用程序的 SAML 单一登录</span><span class="sxs-lookup"><span data-stu-id="3b7b7-119">SAML single sign-on for on-premises applications with Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps)
- [<span data-ttu-id="3b7b7-120">了解并解决 Azure Active Directory 应用程序代理 CORS 问题</span><span class="sxs-lookup"><span data-stu-id="3b7b7-120">Understand and solve Azure Active Directory Application Proxy CORS issues</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#solutions-for-application-proxy-cors-issues)
- [<span data-ttu-id="3b7b7-121">应用程序代理的 Kerberos 约束委派配置疑难解答</span><span class="sxs-lookup"><span data-stu-id="3b7b7-121">Troubleshoot Kerberos constrained delegation configurations for Application Proxy</span></span>](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-back-end-kerberos-constrained-delegation-how-to)