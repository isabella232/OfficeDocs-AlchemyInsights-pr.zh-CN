---
title: 不使用 Exchange 管理中心中的保留策略
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: c9061fa728edaab6575a7b1027783e56739a6d14
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29934982"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="6c417-102">Exchange 管理中心中的保留策略</span><span class="sxs-lookup"><span data-stu-id="6c417-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="6c417-103">**问题：** 新建的或不将 Exchange 管理中心中的更新的保留策略应用于邮箱或不移动到存档邮箱或删除项。</span><span class="sxs-lookup"><span data-stu-id="6c417-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="6c417-104">**根本原因：**</span><span class="sxs-lookup"><span data-stu-id="6c417-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="6c417-p101">这可能是因为**托管文件夹助理**尚未处理用户的邮箱。托管文件夹助理尝试处理七天一次您的基于云的组织中的每个邮箱。如果您更改保留标记或不同的保留策略应用于邮箱，您可以等待，直到托管文件夹帮助处理邮箱，或者您可以运行 Start-managedfolderassistant cmdlet 启动托管文件夹助理处理特定邮箱。运行此 cmdlet 可用于测试或疑难解答保留策略或保留标记设置。有关详细信息，请访问[运行托管文件夹助理](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)。</span><span class="sxs-lookup"><span data-stu-id="6c417-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="6c417-110">**解决方案：** 运行以下命令以启动托管文件夹助理特定邮箱的：</span><span class="sxs-lookup"><span data-stu-id="6c417-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="6c417-p102">这也如果**RetentionHold**已**启用**邮箱发生。如果邮箱已被 RetentionHold 置于，将不会在该时段中处理邮箱的保留策略。有关详细信息时 RetentionHold 设置请参阅：[邮箱保留挂起](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)。</span><span class="sxs-lookup"><span data-stu-id="6c417-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="6c417-114">**解决方案：**</span><span class="sxs-lookup"><span data-stu-id="6c417-114">**Solution:**</span></span>
    
  - <span data-ttu-id="6c417-115">检查[EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)中的特定邮箱的 RetentionHold 设置的状态：</span><span class="sxs-lookup"><span data-stu-id="6c417-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="6c417-116">在特定邮箱上运行以下命令以**禁用**RetentionHold:</span><span class="sxs-lookup"><span data-stu-id="6c417-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="6c417-117">现在，重新运行托管文件夹助理：</span><span class="sxs-lookup"><span data-stu-id="6c417-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="6c417-118">**注意：** 如果邮箱小于 10 MB，托管文件夹助理将不自动处理邮箱。</span><span class="sxs-lookup"><span data-stu-id="6c417-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

