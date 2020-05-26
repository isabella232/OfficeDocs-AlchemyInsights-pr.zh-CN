---
title: 从地址列表中隐藏或取消隐藏 Office 365 组或团队
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: cb3c2819ff7203774511bd0e45633b59a02091ff
ms.sourcegitcommit: e3a1f96200bc58dc8a5b3597cc2600e71c4bd266
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2020
ms.locfileid: "44225341"
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
