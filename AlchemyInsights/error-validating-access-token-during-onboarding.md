---
title: 在桌面分析备前验证访问令牌错误时出现错误
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783541"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="519ec-102">"在桌面 Analytics 载入过程中验证访问令牌时出现错误" 错误</span><span class="sxs-lookup"><span data-stu-id="519ec-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="519ec-103">当身份验证令牌过期时，通常会看到此错误。</span><span class="sxs-lookup"><span data-stu-id="519ec-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="519ec-104">通常情况下，刷新页面会刷新令牌。</span><span class="sxs-lookup"><span data-stu-id="519ec-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="519ec-105">但是，如果对用于机载桌面 Analytics 的帐户应用了任何条件访问策略，则可能会保留此问题。</span><span class="sxs-lookup"><span data-stu-id="519ec-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="519ec-106">您可以在 Azure 门户中查看 Azure AD 登录日志，以查看用于桌面 Analytics 载入的帐户是否存在登录故障。</span><span class="sxs-lookup"><span data-stu-id="519ec-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="519ec-107">有关条件访问的详细信息，请参阅 [Plan a 条件 access 部署](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)。</span><span class="sxs-lookup"><span data-stu-id="519ec-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>