---
title: 解决基于密码的无缝单一登录 (SSO) 问题
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709491"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="ef4ad-102">解决基于密码的无缝单一登录 (SSO) 问题</span><span class="sxs-lookup"><span data-stu-id="ef4ad-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="ef4ad-103">若要了解基于密码的 SSO 的基础，请参阅 [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)基于密码的身份验证。</span><span class="sxs-lookup"><span data-stu-id="ef4ad-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="ef4ad-104">**配置基于密码的 SSO**</span><span class="sxs-lookup"><span data-stu-id="ef4ad-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="ef4ad-105">[配置基于密码的单一登录](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - 本文详细介绍了基于密码的 SSO 选项。</span><span class="sxs-lookup"><span data-stu-id="ef4ad-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="ef4ad-106">如果要添加的应用程序需要自定义配置，并且需要使用基于密码的 SSO，则本文适合您。</span><span class="sxs-lookup"><span data-stu-id="ef4ad-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="ef4ad-107">[为本地应用](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) 配置基于密码的单一登录 - 应用程序代理支持多种单一登录模式。</span><span class="sxs-lookup"><span data-stu-id="ef4ad-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="ef4ad-108">基于密码的登录适用于使用用户名/密码组合进行身份验证的应用程序。</span><span class="sxs-lookup"><span data-stu-id="ef4ad-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="ef4ad-109">为应用程序配置基于密码的登录时，用户必须登录本地应用程序一次。</span><span class="sxs-lookup"><span data-stu-id="ef4ad-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="ef4ad-110">此后，Azure Active Directory 将存储登录信息，并会在用户访问它时自动向应用程序提供此信息。</span><span class="sxs-lookup"><span data-stu-id="ef4ad-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="ef4ad-111">你应该已经使用应用程序代理发布和测试应用。</span><span class="sxs-lookup"><span data-stu-id="ef4ad-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="ef4ad-112">如果没有，请按照使用 Azure [AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) 应用程序代理发布应用程序中的步骤操作，然后继续为 Prem 应用配置基于密码的 SSO。</span><span class="sxs-lookup"><span data-stu-id="ef4ad-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="ef4ad-113">若要对基于密码的 SSO 进行疑难解答，请参阅 Azure AD 中基于密码的单 [一登录疑难解答](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="ef4ad-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
