---
title: 从地址列表中隐藏或取消隐藏 Office 365 组或团队
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 1204b9f45fe34015f72c559f77674e980d28c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47782317"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="190c9-102">从地址列表中隐藏或取消隐藏 Office 365 组或团队</span><span class="sxs-lookup"><span data-stu-id="190c9-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="190c9-103">使用下列 EXO PowerShell 命令，从 Exchange 客户端 (Outlook, OWA) 的地址列表 (GAL) 中隐藏或取消隐藏 Office 365 组/团队：</span><span class="sxs-lookup"><span data-stu-id="190c9-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="190c9-104">使用下列 EXO PowerShell 命令，从 Exchange 客户端 (Outlook, OWA) 中隐藏或取消隐藏 Office 365 组/团队：</span><span class="sxs-lookup"><span data-stu-id="190c9-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="190c9-105">有关详细说明，请参阅 [从 GAL 和 Exchange 客户端中隐藏 Office 365 组](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)。</span><span class="sxs-lookup"><span data-stu-id="190c9-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>
