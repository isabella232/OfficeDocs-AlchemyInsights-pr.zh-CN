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
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926235"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>在MICROSOFT 365 GAL 地址列表中隐藏 (组) 

若要 Microsoft 365从 Exchange 客户端 (（如 Outlook 或 OWA) ）的地址列表 (GAL) 中隐藏) 组，请使用 EXO 命令行管理程序中的以下命令：

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

若要隐藏Microsoft 365组对客户端Exchange，请使用 EXO 命令行管理程序中的以下命令：

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

