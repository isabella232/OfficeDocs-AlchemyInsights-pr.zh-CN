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
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2021
ms.locfileid: "49911971"
---
# <a name="configure-and-extend-token-lifetimes"></a><span data-ttu-id="5bd02-102">配置和延长令牌生存期</span><span class="sxs-lookup"><span data-stu-id="5bd02-102">Configure and extend token lifetimes</span></span>

<span data-ttu-id="5bd02-103">您可以指定由 Microsoft 标识平台颁发的访问、SAML 或 ID 令牌的生存期。</span><span class="sxs-lookup"><span data-stu-id="5bd02-103">You can specify the lifetime of an access, SAML, or ID token issued by Microsoft identity platform.</span></span> <span data-ttu-id="5bd02-104">可以为组织中的所有应用程序、多租户（多组织）应用程序或组织中的特定服务主体设置令牌生存期。</span><span class="sxs-lookup"><span data-stu-id="5bd02-104">You can set token lifetimes for all apps in your organization, for a multi-tenant (multi-organization) application, or for a specific service principal in your organization.</span></span> <span data-ttu-id="5bd02-105">有关更多信息，请阅读[可配置令牌生存期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)。</span><span class="sxs-lookup"><span data-stu-id="5bd02-105">For more info, read [configurable token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).</span></span>

<span data-ttu-id="5bd02-106">例如，阅读[如何配置令牌生存期的示例](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes)。</span><span class="sxs-lookup"><span data-stu-id="5bd02-106">For examples, read [examples of how to configure token lifetimes](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).</span></span>

<span data-ttu-id="5bd02-107">要了解如何在 Azure Active Directory B2C (Azure AD B2C) 中配置令牌的生存期和兼容性，请参阅[在 Azure Active Directory B2C 中配置令牌](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow)。</span><span class="sxs-lookup"><span data-stu-id="5bd02-107">To learn how to configure the lifetime and compatibility of a token in Azure Active Directory B2C (Azure AD B2C), see [Configure tokens in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).</span></span>

<span data-ttu-id="5bd02-108">文章[在 Azure Active Directory B2C 中配置会话行为](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow)描述了 Azure AD B2C 中使用的单一登录 (SSO) 方法，并帮助你在配置策略时选择最合适的 SSO 方法。</span><span class="sxs-lookup"><span data-stu-id="5bd02-108">The article [Configure session behavior in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) describes the single sign-on (SSO) methods used in Azure AD B2C and helps you choose the most appropriate SSO method when configuring your policy.</span></span>

<span data-ttu-id="5bd02-109">**令牌能用多久？有效期是多久？**</span><span class="sxs-lookup"><span data-stu-id="5bd02-109">**How long do tokens last? How long are they valid for?**</span></span>

<span data-ttu-id="5bd02-110">令牌生存期为 1 小时，会话生存期为 24 小时。</span><span class="sxs-lookup"><span data-stu-id="5bd02-110">Token lifetimes are 1 hour and the session lifetime is 24 hours.</span></span> <span data-ttu-id="5bd02-111">这意味着，如果 24 小时内没有任何请求，则需要在请求新令牌之前再次登录。</span><span class="sxs-lookup"><span data-stu-id="5bd02-111">This means that if no requests have been made in 24 hours, you will need to log in again before requesting a new token.</span></span>

> [!NOTE]
> <span data-ttu-id="5bd02-112">2020 年 5 月 30 日之后，新租户将无法使用可配置令牌生存期策略来配置会话和刷新令牌。</span><span class="sxs-lookup"><span data-stu-id="5bd02-112">After May 30, 2020, no new tenant will be able to use Configurable Token Lifetime policy to configure session and refresh tokens.</span></span> <span data-ttu-id="5bd02-113">弃用将在之后的几个月内发生，这意味着我们将停止执行现有会话并刷新令牌策略。</span><span class="sxs-lookup"><span data-stu-id="5bd02-113">The deprecation will happen within several months after that, which means that we will stop honoring existing session and refresh tokens polices.</span></span> <span data-ttu-id="5bd02-114">仍然可以在弃用之后配置访问令牌生存期。</span><span class="sxs-lookup"><span data-stu-id="5bd02-114">You can still configure access token lifetimes after the deprecation.</span></span>






