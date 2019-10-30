---
title: 在地址列表中隐藏/取消隐藏组的说明
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768902"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>隐藏来自地址列表（GAL）的 Office 365 组

若要从 Exchange 客户端（如 Outlook 或 OWA）的地址列表（GAL）中隐藏 Office 365 组，请在 EXO 命令行管理程序中使用以下命令：

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

若要隐藏 Exchange 客户端对 Office 365 组的可见性，请在 EXO 命令行管理程序中使用以下命令：

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

