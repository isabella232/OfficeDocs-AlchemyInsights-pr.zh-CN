---
title: Exchange Online PowerShell 中的微延迟或限制
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 7ab4e7f18b7b8edf08098af8fe9674f66b1b81f4
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947799"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Exchange Online PowerShell 中的微延迟或限制

在 Exchange Online 中运行脚本和 cmdlet 时，可能会看到“已应用微延迟”警告或延迟。 下面是两个相关建议：

- 你可能想要尝试使用 [Exchange Online v2 PowerShell 模块](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)，该模块包含基于 REST API 的 CMDlet，且显著提高了性能。 对于经常使用的大量 Get- CMDlet，这可能是一个很好的解决方案。
- 如果你需要使用 v2 模块中尚未介绍的 CMDlet，请参阅[为大量 Office 365 用户运行 PowerShell cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)，该 cmdlet 讨论如何在 Exchange Online 中绕过预期的 PowerShell 限制。
