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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830023"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="c8f90-102">Exchange Online PowerShell 中的微延迟或限制</span><span class="sxs-lookup"><span data-stu-id="c8f90-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="c8f90-103">在 Exchange Online 中运行脚本和 cmdlet 时，可能会看到“已应用微延迟”警告或延迟。</span><span class="sxs-lookup"><span data-stu-id="c8f90-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="c8f90-104">下面是两个相关建议：</span><span class="sxs-lookup"><span data-stu-id="c8f90-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="c8f90-105">你可能想要尝试使用 [Exchange Online v2 PowerShell 模块](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)，该模块包含基于 REST API 的 CMDlet，且显著提高了性能。</span><span class="sxs-lookup"><span data-stu-id="c8f90-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="c8f90-106">对于经常使用的大量 Get- CMDlet，这可能是一个很好的解决方案。</span><span class="sxs-lookup"><span data-stu-id="c8f90-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="c8f90-107">如果你需要使用 v2 模块中尚未介绍的 CMDlet，请参阅[为大量 Office 365 用户运行 PowerShell cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)，该 cmdlet 讨论如何在 Exchange Online 中绕过预期的 PowerShell 限制。</span><span class="sxs-lookup"><span data-stu-id="c8f90-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
