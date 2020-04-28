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
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908334"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>隐藏来自地址列表（GAL）的 Microsoft 365 组

若要从 Exchange 客户端（如 Outlook 或 OWA）的地址列表（GAL）中隐藏 Microsoft 365 组，请在 EXO 命令行管理程序中使用以下命令：

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

若要隐藏 Microsoft 365 组以使其对 Exchange 客户端可见，请在 EXO 命令行管理程序中使用以下命令：

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

