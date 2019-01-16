---
title: 将电子邮件移动到存档邮箱
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28278029"
---
<span data-ttu-id="dfba3-p101">在遇到存档项目复制到存档邮箱的问题。请确保已执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="dfba3-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="dfba3-p102">确认已启用**存档邮箱**。如果没有，请使用[本文](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes)中的步骤为启用存档邮箱。</span><span class="sxs-lookup"><span data-stu-id="dfba3-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="dfba3-106">在 Exchange 管理中心中，选择**合规性管理**下的**保留标记**中，使用**移动到存档**操作包含所需的**保留时间**创建**保留标记**。</span><span class="sxs-lookup"><span data-stu-id="dfba3-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="dfba3-107">在 Exchange 管理中心中，选择**保留策略**、 创建**保留策略**和将您**移动到存档**保留标记添加到该策略。</span><span class="sxs-lookup"><span data-stu-id="dfba3-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="dfba3-p103">向特定用户的邮箱中[分配将保留策略](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)。将相同的策略将应用于**主要**和**存档**邮箱。</span><span class="sxs-lookup"><span data-stu-id="dfba3-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="dfba3-p104">现在，用户的邮箱应具有将项目移动到存档邮箱的存档策略。可能需要强制托管文件夹助理 (MFA) 运行，并将新设置应用于用户的邮箱。运行下面的命令时[连接到 EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)启动托管文件夹助理特定邮箱的：</span><span class="sxs-lookup"><span data-stu-id="dfba3-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="dfba3-113">要设置存档策略的详细信息，请参阅[Set up 邮箱的存档和删除策略](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)。</span><span class="sxs-lookup"><span data-stu-id="dfba3-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

