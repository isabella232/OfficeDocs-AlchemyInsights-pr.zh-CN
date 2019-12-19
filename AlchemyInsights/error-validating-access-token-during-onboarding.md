---
title: 在桌面分析备前验证访问令牌错误时出现错误
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741124"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="e04aa-102">"在桌面 Analytics 载入过程中验证访问令牌时出现错误" 错误</span><span class="sxs-lookup"><span data-stu-id="e04aa-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="e04aa-103">当身份验证令牌过期时，通常会看到此错误。</span><span class="sxs-lookup"><span data-stu-id="e04aa-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="e04aa-104">通常情况下，刷新页面会刷新令牌。</span><span class="sxs-lookup"><span data-stu-id="e04aa-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="e04aa-105">但是，如果对用于机载桌面 Analytics 的帐户应用了任何条件访问策略，则可能会保留此问题。</span><span class="sxs-lookup"><span data-stu-id="e04aa-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="e04aa-106">您可以在 Azure 门户中查看 Azure AD 登录日志，以查看用于桌面 Analytics 载入的帐户是否存在登录故障。</span><span class="sxs-lookup"><span data-stu-id="e04aa-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="e04aa-107">有关条件访问的详细信息，请参阅[Plan a 条件 access 部署](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)。</span><span class="sxs-lookup"><span data-stu-id="e04aa-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>