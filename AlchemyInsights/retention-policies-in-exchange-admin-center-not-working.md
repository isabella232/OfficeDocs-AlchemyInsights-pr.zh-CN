---
title: 不使用 Exchange 管理中心中的保留策略
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28276958"
---
 **问题：** 新建的或不将 Exchange 管理中心中的更新的保留策略应用于邮箱或不移动到存档邮箱或删除项。 
  
 **根本原因：**
  
- 这可能是因为**托管文件夹助理**尚未处理用户的邮箱。托管文件夹助理尝试处理七天一次您的基于云的组织中的每个邮箱。如果您更改保留标记或不同的保留策略应用于邮箱，您可以等待，直到托管文件夹帮助处理邮箱，或者您可以运行 Start-managedfolderassistant cmdlet 启动托管文件夹助理处理特定邮箱。运行此 cmdlet 可用于测试或疑难解答保留策略或保留标记设置。有关详细信息，请访问[运行托管文件夹助理](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)。
    
  - **解决方案：** 运行以下命令以启动托管文件夹助理特定邮箱的： 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- 这也如果**RetentionHold**已**启用**邮箱发生。如果邮箱已被 RetentionHold 置于，将不会在该时段中处理邮箱的保留策略。有关详细信息时 RetentionHold 设置请参阅：[邮箱保留挂起](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)。
    
    **解决方案：**
    
  - 检查[EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)中的特定邮箱的 RetentionHold 设置的状态：
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - 在特定邮箱上运行以下命令以**禁用**RetentionHold: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - 现在，重新运行托管文件夹助理：
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **注意：** 如果邮箱小于 10 MB，托管文件夹助理将不自动处理邮箱。 
  

