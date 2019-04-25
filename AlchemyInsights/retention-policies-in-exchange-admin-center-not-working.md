---
title: Exchange Admin Center 中的保留策略无法正常工作
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
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32371288"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="1a20e-102">Exchange 管理中心中的保留策略</span><span class="sxs-lookup"><span data-stu-id="1a20e-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="1a20e-103">**问题:** Exchange 管理中心中新创建或更新的保留策略不会应用于邮箱或项目不会移动到存档邮箱或将其删除。</span><span class="sxs-lookup"><span data-stu-id="1a20e-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="1a20e-104">**根本原因:**</span><span class="sxs-lookup"><span data-stu-id="1a20e-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="1a20e-105">这可能是因为**托管文件夹助理**尚未处理用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="1a20e-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="1a20e-106">托管文件夹助理每七天尝试处理一次基于云的组织中的每个邮箱。</span><span class="sxs-lookup"><span data-stu-id="1a20e-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="1a20e-107">如果您更改保留标记或对邮箱应用不同的保留策略, 则可以等待托管文件夹帮助处理邮箱, 也可以运行 start-managedfolderassistant cmdlet 启动托管文件夹助理以处理特定的信箱.</span><span class="sxs-lookup"><span data-stu-id="1a20e-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="1a20e-108">运行此 cmdlet 对于测试或排除保留策略或保留标记设置的故障很有用。</span><span class="sxs-lookup"><span data-stu-id="1a20e-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="1a20e-109">有关详细信息, 请参阅[运行托管文件夹助理](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)。</span><span class="sxs-lookup"><span data-stu-id="1a20e-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="1a20e-110">**解决方案:** 运行以下命令以启动特定邮箱的托管文件夹助理:</span><span class="sxs-lookup"><span data-stu-id="1a20e-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="1a20e-111">如果已在邮箱上启用**RetentionHold** , 也\*\*\*\* 可能出现此情况。</span><span class="sxs-lookup"><span data-stu-id="1a20e-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="1a20e-112">如果已将邮箱放在 RetentionHold 中, 则邮箱中的保留策略将不会在该时间进行处理。</span><span class="sxs-lookup"><span data-stu-id="1a20e-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="1a20e-113">有关 RetentionHold 设置的详细 informaton, 请参阅:[邮箱保留挂起](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)。</span><span class="sxs-lookup"><span data-stu-id="1a20e-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="1a20e-114">**办法**</span><span class="sxs-lookup"><span data-stu-id="1a20e-114">**Solution:**</span></span>
    
  - <span data-ttu-id="1a20e-115">检查[EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)中特定邮箱上的 RetentionHold 设置的状态:</span><span class="sxs-lookup"><span data-stu-id="1a20e-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="1a20e-116">运行以下命令, 在特定邮箱上**禁用**RetentionHold:</span><span class="sxs-lookup"><span data-stu-id="1a20e-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="1a20e-117">现在, 重新运行托管文件夹助理:</span><span class="sxs-lookup"><span data-stu-id="1a20e-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="1a20e-118">**注意:** 如果邮箱小于 10 MB, 则托管文件夹助理将不会自动处理邮箱。</span><span class="sxs-lookup"><span data-stu-id="1a20e-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

