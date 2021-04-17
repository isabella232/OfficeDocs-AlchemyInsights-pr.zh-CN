---
title: 使用 cmdlet 恢复已删除的项目
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835801"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="63204-102">使用 cmdlet 恢复已删除的项目</span><span class="sxs-lookup"><span data-stu-id="63204-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="63204-103">使用 [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet 查看邮箱中的已删除项目。</span><span class="sxs-lookup"><span data-stu-id="63204-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="63204-104">找到已删除的项目后，可使用 [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet 还原它们。</span><span class="sxs-lookup"><span data-stu-id="63204-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="63204-105">请参阅 [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) 的完整详细信息。</span><span class="sxs-lookup"><span data-stu-id="63204-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="63204-106">你必须先分配到“邮箱导入导出”角色，才能运行此 cmdlet。</span><span class="sxs-lookup"><span data-stu-id="63204-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="63204-107">有关更多详细信息，请参阅 [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="63204-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
