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
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="9e518-102">隐藏来自地址列表（GAL）的 Microsoft 365 组</span><span class="sxs-lookup"><span data-stu-id="9e518-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="9e518-103">若要从 Exchange 客户端（如 Outlook 或 OWA）的地址列表（GAL）中隐藏 Microsoft 365 组，请在 EXO 命令行管理程序中使用以下命令：</span><span class="sxs-lookup"><span data-stu-id="9e518-103">To hide an Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="9e518-104">若要隐藏 Microsoft 365 组以使其对 Exchange 客户端可见，请在 EXO 命令行管理程序中使用以下命令：</span><span class="sxs-lookup"><span data-stu-id="9e518-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

