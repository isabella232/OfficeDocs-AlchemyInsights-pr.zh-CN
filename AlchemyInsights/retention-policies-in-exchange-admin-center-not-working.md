---
title: Exchange Admin Center 中的保留策略无法正常工作
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502597"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="d794d-102">Exchange 管理中心中的保留策略</span><span class="sxs-lookup"><span data-stu-id="d794d-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="d794d-103">**问题：** Exchange 管理中心中新创建或更新的保留策略不会应用于邮箱或项目不会移动到存档邮箱或将其删除。</span><span class="sxs-lookup"><span data-stu-id="d794d-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="d794d-104">**根本原因：**</span><span class="sxs-lookup"><span data-stu-id="d794d-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="d794d-105">这可能是因为**托管文件夹助理**尚未处理用户的邮箱。</span><span class="sxs-lookup"><span data-stu-id="d794d-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="d794d-106">托管文件夹助理每七天尝试处理一次基于云的组织中的每个邮箱。</span><span class="sxs-lookup"><span data-stu-id="d794d-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="d794d-107">如果您更改保留标记或向邮箱应用不同的保留策略，则可以等待托管文件夹帮助处理邮箱，也可以运行 Start-managedfolderassistant cmdlet 以启动托管文件夹助理来处理特定邮箱。</span><span class="sxs-lookup"><span data-stu-id="d794d-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="d794d-108">运行此 cmdlet 对于测试或排除保留策略或保留标记设置的故障很有用。</span><span class="sxs-lookup"><span data-stu-id="d794d-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="d794d-109">有关详细信息，请参阅[运行托管文件夹助理](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)。</span><span class="sxs-lookup"><span data-stu-id="d794d-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="d794d-110">**解决方案：** 运行以下命令以启动特定邮箱的托管文件夹助理：</span><span class="sxs-lookup"><span data-stu-id="d794d-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="d794d-111">如果已在邮箱上启用**RetentionHold** ，也**enabled**可能出现此情况。</span><span class="sxs-lookup"><span data-stu-id="d794d-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="d794d-112">如果已将邮箱放在 RetentionHold 中，则邮箱中的保留策略将不会在该时间进行处理。</span><span class="sxs-lookup"><span data-stu-id="d794d-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="d794d-113">有关 RetentionHold 设置的详细 informaton，请参阅：[邮箱保留挂起](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)。</span><span class="sxs-lookup"><span data-stu-id="d794d-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="d794d-114">**办法**</span><span class="sxs-lookup"><span data-stu-id="d794d-114">**Solution:**</span></span>
    
  - <span data-ttu-id="d794d-115">检查[EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)中特定邮箱上的 RetentionHold 设置的状态：</span><span class="sxs-lookup"><span data-stu-id="d794d-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="d794d-116">运行以下命令，在特定邮箱上**禁用**RetentionHold：</span><span class="sxs-lookup"><span data-stu-id="d794d-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="d794d-117">现在，重新运行托管文件夹助理：</span><span class="sxs-lookup"><span data-stu-id="d794d-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="d794d-118">**注意：** 如果邮箱小于 10 MB，则托管文件夹助理将不会自动处理邮箱。</span><span class="sxs-lookup"><span data-stu-id="d794d-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="d794d-119">有关 Exchange 管理中心中的保留策略的详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="d794d-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="d794d-120">保留标记和保留策略</span><span class="sxs-lookup"><span data-stu-id="d794d-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="d794d-121">将保留策略应用于邮箱</span><span class="sxs-lookup"><span data-stu-id="d794d-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="d794d-122">添加或删除保留标记</span><span class="sxs-lookup"><span data-stu-id="d794d-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="d794d-123">如何识别为邮箱设置的保留类型</span><span class="sxs-lookup"><span data-stu-id="d794d-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
