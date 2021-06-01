---
title: Exchange Online PowerShell 中的微延迟或限制
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702116"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="39bd6-102">Exchange Online PowerShell 中的微延迟或限制</span><span class="sxs-lookup"><span data-stu-id="39bd6-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="39bd6-103">在 Exchange Online 中运行脚本和 cmdlet 时，可能会看到“已应用微延迟”警告或延迟。</span><span class="sxs-lookup"><span data-stu-id="39bd6-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="39bd6-104">下面是如何解决此问题的一些建议：</span><span class="sxs-lookup"><span data-stu-id="39bd6-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="39bd6-105">请运行诊断，以放宽租户的 PowerShell 限制策略。</span><span class="sxs-lookup"><span data-stu-id="39bd6-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="39bd6-106">此解决方案将解决大多数问题。</span><span class="sxs-lookup"><span data-stu-id="39bd6-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="39bd6-107">如果问题未解决，请使用 [Exchange Online v2 PowerShell 模块](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)，该模块包含基于 REST API 的 CMDlet，且显著提高了性能。</span><span class="sxs-lookup"><span data-stu-id="39bd6-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="39bd6-108">对于经常使用的大量 Get- CMDlet，这可能是一个很好的解决方案。</span><span class="sxs-lookup"><span data-stu-id="39bd6-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="39bd6-109">如果需要使用 v2 模块中未包含的 CMDlet，请参阅 [在 Office 365 中为大量用户运行 PowerShell cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)，其中讨论了如何在 Exchange Online 中绕过 PowerShell 限制。</span><span class="sxs-lookup"><span data-stu-id="39bd6-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
