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
ms.openlocfilehash: 6753dcb375ea5e19b01c4350b61aa8904aa102112df175a3f70281d18a634dbf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098556"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Exchange Online PowerShell 中的微延迟或限制

在 Exchange Online 中运行脚本和 cmdlet 时，可能会看到“已应用微延迟”警告或延迟。 下面是如何解决此问题的一些建议：

- 请运行诊断，以放宽租户的 PowerShell 限制策略。 此解决方案将解决大多数问题。
- 如果问题未解决，请使用 [Exchange Online v2 PowerShell 模块](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)，该模块包含基于 REST API 的 CMDlet，且显著提高了性能。 对于经常使用的大量 Get- CMDlet，这可能是一个很好的解决方案。
- 如果需要使用 v2 模块中未包含的 CMDlet，请参阅 [在 Office 365 中为大量用户运行 PowerShell cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)，其中讨论了如何在 Exchange Online 中绕过 PowerShell 限制。
