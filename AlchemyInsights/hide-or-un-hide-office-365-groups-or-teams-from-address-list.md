---
title: 从地址列表中隐藏或取消隐藏 Office 365 组或团队
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
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811446"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>从地址列表中隐藏或取消隐藏 Office 365 组或团队

使用下列 EXO PowerShell 命令，从 Exchange 客户端 (Outlook, OWA) 的地址列表 (GAL) 中隐藏或取消隐藏 Office 365 组/团队：

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

使用下列 EXO PowerShell 命令，从 Exchange 客户端 (Outlook, OWA) 中隐藏或取消隐藏 Office 365 组/团队：

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- 有关详细说明，请参阅 [从 GAL 和 Exchange 客户端中隐藏 Office 365 组](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)。
