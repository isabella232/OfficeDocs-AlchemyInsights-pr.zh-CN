---
title: 还原已删除的邮箱
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 18e56305b60469422a154ffa1b097c238baaae16
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764646"
---
# <a name="restore-a-deleted-mailbox"></a><span data-ttu-id="7d7cd-102">还原已删除的邮箱</span><span class="sxs-lookup"><span data-stu-id="7d7cd-102">Restore a deleted mailbox</span></span>

<span data-ttu-id="7d7cd-103">当用户丢失 Exchange Online 许可证时，其邮箱将保留30天，并且可以通过将许可证重新分配给用户来进行恢复。</span><span class="sxs-lookup"><span data-stu-id="7d7cd-103">When a user loses an Exchange Online license, their mailbox is retained for 30 days and can be recovered by simply re-assigning the license to the user.</span></span>
  
 <span data-ttu-id="7d7cd-104">*这将仅在30天内有效。*</span><span class="sxs-lookup"><span data-stu-id="7d7cd-104">*This will work only within 30 days.*</span></span>  
  
1. <span data-ttu-id="7d7cd-105">在 Microsoft 365 管理中心，转到 "**用户** \> **活动用户**" 页。</span><span class="sxs-lookup"><span data-stu-id="7d7cd-105">In the Microsoft 365 admin center, go to the **Users** \> **Active users** page.</span></span> <span data-ttu-id="7d7cd-106">选择 "有问题的用户"。</span><span class="sxs-lookup"><span data-stu-id="7d7cd-106">Select the user in question.</span></span>

2. <span data-ttu-id="7d7cd-107">在 "**许可证和应用**" 选项卡上，分配 Exchange Online 许可证并选择 "**保存更改**"。</span><span class="sxs-lookup"><span data-stu-id="7d7cd-107">On the **Licenses and Apps** tab, assign the Exchange Online license and select **Save changes**.</span></span>

<span data-ttu-id="7d7cd-108">如果尝试恢复共享邮箱，它也可以恢复30天。</span><span class="sxs-lookup"><span data-stu-id="7d7cd-108">If you are trying to recover a Shared mailbox, it is also recoverable for 30 days.</span></span> <span data-ttu-id="7d7cd-109">你可以在**用户** \> **删除的用户**下找到它们;共享邮箱不需要许可证。</span><span class="sxs-lookup"><span data-stu-id="7d7cd-109">You can find them under **Users** \> **Deleted users**; shared mailboxes do not require a license.</span></span> <span data-ttu-id="7d7cd-110">如果您意识到您需要还原已删除的用户，请参阅[还原用户](https://docs.microsoft.com/office365/admin/add-users/restore-user)。</span><span class="sxs-lookup"><span data-stu-id="7d7cd-110">If you realize that you need to restore a deleted user, please see [Restore a user](https://docs.microsoft.com/office365/admin/add-users/restore-user).</span></span>
  