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
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579999"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="f2d1f-102">隐藏来自地址列表（GAL）的 Microsoft 365 组</span><span class="sxs-lookup"><span data-stu-id="f2d1f-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="f2d1f-103">若要从 Exchange 客户端（如 Outlook 或 OWA）的地址列表（GAL）中隐藏 Microsoft 365 组，请在 EXO 命令行管理程序中使用以下命令：</span><span class="sxs-lookup"><span data-stu-id="f2d1f-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="f2d1f-104">若要隐藏 Microsoft 365 组以使其对 Exchange 客户端可见，请在 EXO 命令行管理程序中使用以下命令：</span><span class="sxs-lookup"><span data-stu-id="f2d1f-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

