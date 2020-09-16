---
title: 使用 cmdlet 恢复已删除的项目
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
- "1800008"
- "5718"
ms.openlocfilehash: 91a9bcf75b13881b903a1d3b6f2da53f65811c9c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741293"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="7f0ed-102">使用 cmdlet 恢复已删除的项目</span><span class="sxs-lookup"><span data-stu-id="7f0ed-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="7f0ed-103">使用 [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet 查看邮箱中的已删除项目。</span><span class="sxs-lookup"><span data-stu-id="7f0ed-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="7f0ed-104">找到已删除的项目后，可使用 [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet 还原它们。</span><span class="sxs-lookup"><span data-stu-id="7f0ed-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="7f0ed-105">请参阅 [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) 的完整详细信息。</span><span class="sxs-lookup"><span data-stu-id="7f0ed-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="7f0ed-106">你必须先分配到“邮箱导入导出”角色，才能运行此 cmdlet。</span><span class="sxs-lookup"><span data-stu-id="7f0ed-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="7f0ed-107">有关更多详细信息，请参阅 [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="7f0ed-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
