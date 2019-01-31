---
title: 1336 RecoverableItems 文件夹已满
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: b8b3e5389778b3aff0fbe2f6506ba2b2fc3abc7e
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655657"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="b5da3-102">可恢复邮件文件夹已满</span><span class="sxs-lookup"><span data-stu-id="b5da3-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="b5da3-p101">Office 365 中的 Exchange Online 邮箱，可恢复邮件文件夹的默认存储限制为 30 GB。如果邮箱置于诉讼保留电子数据展示保留或已分配给 Office 365 保留策略，可恢复邮件文件夹的存储限制会自动增加到 100 GB。</span><span class="sxs-lookup"><span data-stu-id="b5da3-p101">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB. The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>
  
<span data-ttu-id="b5da3-105">当可恢复邮件文件夹达到的存储限制时，邮箱功能将受到影响以下方式：</span><span class="sxs-lookup"><span data-stu-id="b5da3-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>
  
- <span data-ttu-id="b5da3-106">用户无法从邮箱中删除项目。</span><span class="sxs-lookup"><span data-stu-id="b5da3-106">The user can't delete items from the mailbox.</span></span>
    
- <span data-ttu-id="b5da3-107">托管文件夹助理无法基于保留标记或托管文件夹设置删除项目。</span><span class="sxs-lookup"><span data-stu-id="b5da3-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>
    
- <span data-ttu-id="b5da3-108">已启用的单个项目恢复或置于保持状态的邮箱，写入时复制页保护过程无法保持用户编辑的项目的版本。</span><span class="sxs-lookup"><span data-stu-id="b5da3-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>
    
- <span data-ttu-id="b5da3-109">具有邮箱审核日志记录启用的邮箱，可以在可恢复邮件文件夹中的审核子文件夹中保存没有邮箱审核日志条目。</span><span class="sxs-lookup"><span data-stu-id="b5da3-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>
    
<span data-ttu-id="b5da3-p102">对于不是置于保持状态的邮箱，管理员可以使用`Search-Mailbox -SearchDumpsterOnly -DeleteContent`命令在 Exchange Online PowerShell 中删除可恢复邮件文件夹中的项目。有关详细信息，请参阅以下主题：</span><span class="sxs-lookup"><span data-stu-id="b5da3-p102">For mailboxes that aren't on hold, admins can use the  `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder. For more information, see the following topics:</span></span> 
  
- [<span data-ttu-id="b5da3-112">搜索和删除邮件</span><span class="sxs-lookup"><span data-stu-id="b5da3-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [<span data-ttu-id="b5da3-113">Search-Mailbox</span><span class="sxs-lookup"><span data-stu-id="b5da3-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
<span data-ttu-id="b5da3-p103">对于处于保持状态的邮箱，管理员必须删除保留，他们可以从可恢复邮件文件夹的已删除的项目之前。有关详细信息，请参阅[删除在可恢复项目文件夹中的基于云的邮箱的保留的项目](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)。</span><span class="sxs-lookup"><span data-stu-id="b5da3-p103">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder. For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>
  
<span data-ttu-id="b5da3-p104">为了帮助防止成为完整可恢复邮件文件夹，管理员可以提高可恢复的项目文件夹上邮箱保留和设置将项目从可恢复邮件文件夹移动到用户的存档邮箱保留策略的存储限制邮箱。请参阅[提高可恢复的项目上的邮箱配额保留](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)。</span><span class="sxs-lookup"><span data-stu-id="b5da3-p104">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox. See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
  

