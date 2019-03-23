---
title: 1336 RecoverableItems 文件夹已满
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: a048949d5284d018303d03aad26cdf26eee2fb5c
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776387"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="33b1e-102">"可恢复的项目" 文件夹已满</span><span class="sxs-lookup"><span data-stu-id="33b1e-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="33b1e-103">对于 Office 365 中的 Exchange Online 邮箱, "可恢复的项目" 文件夹的默认存储限制为 30 GB。</span><span class="sxs-lookup"><span data-stu-id="33b1e-103">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="33b1e-104">如果将邮箱置于诉讼保留、电子数据展示保留或分配到 Office 365 保留策略, 则 "可恢复的项目" 文件夹的存储限制将自动增加到 100 GB。</span><span class="sxs-lookup"><span data-stu-id="33b1e-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>
  
<span data-ttu-id="33b1e-105">当 "可恢复的项目" 文件夹达到存储限制时, 邮箱功能将受到以下几种影响:</span><span class="sxs-lookup"><span data-stu-id="33b1e-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>
  
- <span data-ttu-id="33b1e-106">用户不能删除邮箱中的项目。</span><span class="sxs-lookup"><span data-stu-id="33b1e-106">The user can't delete items from the mailbox.</span></span>
    
- <span data-ttu-id="33b1e-107">托管文件夹助理无法基于保留标记或托管文件夹设置删除项目。</span><span class="sxs-lookup"><span data-stu-id="33b1e-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>
    
- <span data-ttu-id="33b1e-108">对于启用了单个项目恢复或置于保留状态的邮箱, "写入时复制" 页面保护过程无法维护用户编辑的项目的版本。</span><span class="sxs-lookup"><span data-stu-id="33b1e-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>
    
- <span data-ttu-id="33b1e-109">对于启用了邮箱审核日志记录的邮箱, 不能将邮箱审核日志条目保存在 "可恢复的项目" 文件夹的 "审核" 子文件夹中。</span><span class="sxs-lookup"><span data-stu-id="33b1e-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>
    
<span data-ttu-id="33b1e-110">对于不处于保留状态的邮箱, 管理员可以使用`Search-Mailbox -SearchDumpsterOnly -DeleteContent` Exchange Online PowerShell 中的命令删除 "可恢复的项目" 文件夹中的项目。</span><span class="sxs-lookup"><span data-stu-id="33b1e-110">For mailboxes that aren't on hold, admins can use the  `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="33b1e-111">有关详细信息，请参阅下列主题：</span><span class="sxs-lookup"><span data-stu-id="33b1e-111">For more information, see the following topics:</span></span> 
  
- [<span data-ttu-id="33b1e-112">搜索和删除邮件</span><span class="sxs-lookup"><span data-stu-id="33b1e-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)
    
- [<span data-ttu-id="33b1e-113">搜索-邮箱</span><span class="sxs-lookup"><span data-stu-id="33b1e-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)
    
<span data-ttu-id="33b1e-114">对于处于保留状态的邮箱, 管理员必须先删除保留, 然后才能从 "可恢复的项目" 文件夹中删除项目。</span><span class="sxs-lookup"><span data-stu-id="33b1e-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="33b1e-115">有关详细信息, 请参阅[在保留时, 删除基于云的邮箱的 "可恢复的项目" 文件夹中的项目](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)。</span><span class="sxs-lookup"><span data-stu-id="33b1e-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>
  
<span data-ttu-id="33b1e-116">为了帮助防止 "可恢复的项目" 文件夹变满, 管理员可以增加保留邮箱的 "可恢复的项目" 文件夹的存储限制, 并设置将项目从 "可恢复的项目" 文件夹移动到用户存档的邮箱保留策略信箱.</span><span class="sxs-lookup"><span data-stu-id="33b1e-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="33b1e-117">请参阅[增大保留邮箱的可恢复邮件配额](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold)。</span><span class="sxs-lookup"><span data-stu-id="33b1e-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
  

