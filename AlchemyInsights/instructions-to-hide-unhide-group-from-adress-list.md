---
title: 从地址列表中隐藏/取消隐藏组的说明
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
- "1200024"
- "3161"
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831868"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>将 Microsoft 365 组从地址列表 (GAL) 

若要将 Microsoft 365 组从 Exchange 客户端 (GAL) 地址列表中隐藏 (如 Outlook 或 OWA) ，请使用 EXO 命令行管理程序中的以下命令：

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

若要隐藏对 Exchange 客户端可见的 Microsoft 365 组，请使用 EXO 命令行管理程序中的以下命令：

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

