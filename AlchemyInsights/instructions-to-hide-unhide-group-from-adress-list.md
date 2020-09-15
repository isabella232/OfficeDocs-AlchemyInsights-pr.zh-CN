---
title: 在地址列表中隐藏/取消隐藏组的说明
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662999"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="42005-102">将 Microsoft 365 组从地址列表中隐藏 (GAL) </span><span class="sxs-lookup"><span data-stu-id="42005-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="42005-103">若要将 Microsoft 365 组从地址列表中隐藏 (GAL) 的 Exchange 客户端 (如 Outlook 或 OWA) ，请在 EXO 命令行管理程序中使用以下命令：</span><span class="sxs-lookup"><span data-stu-id="42005-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="42005-104">若要隐藏 Microsoft 365 组以使其对 Exchange 客户端可见，请在 EXO 命令行管理程序中使用以下命令：</span><span class="sxs-lookup"><span data-stu-id="42005-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

