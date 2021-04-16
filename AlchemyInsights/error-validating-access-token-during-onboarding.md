---
title: 在桌面分析启动期间验证访问令牌错误时出错
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813678"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="c2ff1-102">桌面分析载入期间出现"验证访问令牌时出错"错误</span><span class="sxs-lookup"><span data-stu-id="c2ff1-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="c2ff1-103">通常在身份验证令牌过期时观察到此错误。</span><span class="sxs-lookup"><span data-stu-id="c2ff1-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="c2ff1-104">通常，刷新页面会刷新令牌。</span><span class="sxs-lookup"><span data-stu-id="c2ff1-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="c2ff1-105">但是，如果存在应用于用于板载桌面分析的帐户的任何条件访问策略，则此问题可能仍然存在。</span><span class="sxs-lookup"><span data-stu-id="c2ff1-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="c2ff1-106">你可以查看 Azure 门户中的 Azure AD 登录日志，以查看用于桌面分析载入的帐户是否有登录失败。</span><span class="sxs-lookup"><span data-stu-id="c2ff1-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="c2ff1-107">有关条件访问详细信息，请访问 [规划条件访问部署](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)。</span><span class="sxs-lookup"><span data-stu-id="c2ff1-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>