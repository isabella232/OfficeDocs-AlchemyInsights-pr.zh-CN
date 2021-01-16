---
title: 应用代理配置
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876534"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="49bd0-102">应用代理配置</span><span class="sxs-lookup"><span data-stu-id="49bd0-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="49bd0-103">若要了解如何在 Azure AD 中配置应用程序代理应用程序以将本地应用程序公开到云中，请参阅 [如何配置应用程序代理应用程序](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)。</span><span class="sxs-lookup"><span data-stu-id="49bd0-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="49bd0-104">SSO (单一) 允许用户访问应用程序，而无需多次进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="49bd0-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="49bd0-105">它允许针对 Azure Active Directory 在云中执行单一身份验证，并允许服务或连接器模拟用户，以从应用程序完成任何其他身份验证挑战。</span><span class="sxs-lookup"><span data-stu-id="49bd0-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="49bd0-106">若要了解更多信息，请参阅 [如何配置应用程序代理应用程序的单一登录](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)。</span><span class="sxs-lookup"><span data-stu-id="49bd0-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="49bd0-107">使用 [本文可](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) 解决用户创建新应用程序代理应用程序时面临的常见问题。</span><span class="sxs-lookup"><span data-stu-id="49bd0-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="49bd0-108">如果在为应用程序设置后端身份验证时遇到问题，您可能需要解决 [应用程序代理的 Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) 约束委派配置问题，或按照有关使用 [PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) 配置应用程序的指南解决问题。</span><span class="sxs-lookup"><span data-stu-id="49bd0-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
