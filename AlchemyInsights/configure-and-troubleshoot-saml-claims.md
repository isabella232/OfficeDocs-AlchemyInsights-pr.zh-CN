---
title: 配置和疑难解答 SAML 声明
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
- "7799"
- "9004356"
ms.openlocfilehash: 306d2f451856a66f06447e3acd73e065da71cd64
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886780"
---
# <a name="configure-and-troubleshoot-saml-claims"></a><span data-ttu-id="9aaae-102">配置和疑难解答 SAML 声明</span><span class="sxs-lookup"><span data-stu-id="9aaae-102">Configure and troubleshoot SAML claims</span></span>

<span data-ttu-id="9aaae-103">配置和疑难解答 SAML 声明：</span><span class="sxs-lookup"><span data-stu-id="9aaae-103">To configure and troubleshoot SAML claims:</span></span>

1. <span data-ttu-id="9aaae-104">按照[这篇文章](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)中罗列的步骤来配置在企业应用 SAML 令牌中提出的角色声明。</span><span class="sxs-lookup"><span data-stu-id="9aaae-104">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) to configure the role claim issued in the SAML token for enterprise applications.</span></span>
2. <span data-ttu-id="9aaae-105">按照[这篇文章](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)中的步骤来自定义在企业应用 SAML 令牌中提出的声明。</span><span class="sxs-lookup"><span data-stu-id="9aaae-105">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization) to customize claims issued in the SAML token for enterprise applications.</span></span>
3. <span data-ttu-id="9aaae-106">按照[这篇文章](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)中的步骤来自定义在租户中具体应用的令牌中发出的声明。</span><span class="sxs-lookup"><span data-stu-id="9aaae-106">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) to customize claims emitted in tokens for a specific app in a tenant.</span></span>
4. <span data-ttu-id="9aaae-107">阅读[这篇文章](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications)来了解如何在应用程序代理中使用声明感知的应用。</span><span class="sxs-lookup"><span data-stu-id="9aaae-107">Read [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) to understand working with claims-aware apps in Application Proxy.</span></span>