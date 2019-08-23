---
title: 还原已删除的邮箱
ms.author: pebaum
author: pebaum
ms.date: 9/12/2017
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "360"
- "3500005"
search.appverid:
- MOE150
- MED150
- MBS150
ms.assetid: e6112a76-bbb6-4c22-b2e6-690b004d92d4
ms.openlocfilehash: 9fc1980b5c1d5a0bd9df032b14e2010b7f0d5873
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551837"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="8aa3c-102">还原已删除的邮箱</span><span class="sxs-lookup"><span data-stu-id="8aa3c-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="8aa3c-103">当用户丢失其 Exchange Online 许可证时, 其邮箱将保留30天, 并且可以通过将许可证重新分配给用户来进行恢复。</span><span class="sxs-lookup"><span data-stu-id="8aa3c-103">When the user loses its Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="8aa3c-104">*这将仅在30天内有效。*</span><span class="sxs-lookup"><span data-stu-id="8aa3c-104">*This will work only within 30 days.*</span></span>  <span data-ttu-id="8aa3c-105">在管理门户中, 转到:</span><span class="sxs-lookup"><span data-stu-id="8aa3c-105">In the Admin Portal, go to:</span></span>
  
1. <span data-ttu-id="8aa3c-106">**用户**\> **活动**用户。</span><span class="sxs-lookup"><span data-stu-id="8aa3c-106">**Users** \> **Active** users.</span></span> <span data-ttu-id="8aa3c-107">选择 "有问题的用户"。</span><span class="sxs-lookup"><span data-stu-id="8aa3c-107">Select the user in question.</span></span>

2. <span data-ttu-id="8aa3c-108">按 "**编辑**" 修改产品许可证</span><span class="sxs-lookup"><span data-stu-id="8aa3c-108">Press **Edit** to modify Product licenses</span></span>

3. <span data-ttu-id="8aa3c-109">分配 Exchange Online 许可证并按 "**保存**"</span><span class="sxs-lookup"><span data-stu-id="8aa3c-109">Assign the Exchange Online license and press **Save**</span></span>

<span data-ttu-id="8aa3c-110">如果尝试恢复共享邮箱, 它也可以恢复30天。</span><span class="sxs-lookup"><span data-stu-id="8aa3c-110">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="8aa3c-111">你可以在**用户** \> **删除**的用户下找到它们;共享邮箱不需要许可证。</span><span class="sxs-lookup"><span data-stu-id="8aa3c-111">You can find them under **Users** \> **Deleted** users; shared mailboxes do not require a license.</span></span> <span data-ttu-id="8aa3c-112">如果您意识到您需要还原已删除的用户, 请参阅[在 Office 365 中还原用户](https://docs.microsoft.com/office365/admin/add-users/restore-user)。</span><span class="sxs-lookup"><span data-stu-id="8aa3c-112">If you realize that you need to restore a deleted user, please see [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span></span>
  