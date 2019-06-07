---
title: Exchange Admin Center 中的保留策略无法正常工作
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 56c2bea5e205358d0ef29fa937e36a88ffc46a1e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761572"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange 管理中心中的保留策略

 **问题:** Exchange 管理中心中新创建或更新的保留策略不会应用于邮箱或项目不会移动到存档邮箱或将其删除。 
  
 **根本原因:**
  
- 这可能是因为**托管文件夹助理**尚未处理用户的邮箱。 托管文件夹助理每七天尝试处理一次基于云的组织中的每个邮箱。 如果您更改保留标记或对邮箱应用不同的保留策略, 则可以等待托管文件夹帮助处理邮箱, 也可以运行 Start-managedfolderassistant cmdlet 启动托管文件夹助理以处理特定的信箱. 运行此 cmdlet 对于测试或排除保留策略或保留标记设置的故障很有用。 有关详细信息, 请参阅[运行托管文件夹助理](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)。
    
  - **解决方案:** 运行以下命令以启动特定邮箱的托管文件夹助理: 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- 如果已在邮箱上启用**RetentionHold** , 也**** 可能出现此情况。 如果已将邮箱放在 RetentionHold 中, 则邮箱中的保留策略将不会在该时间进行处理。 有关 RetentionHold 设置的详细 informaton, 请参阅:[邮箱保留挂起](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)。
    
    **办法**
    
  - 检查[EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)中特定邮箱上的 RetentionHold 设置的状态:
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - 运行以下命令, 在特定邮箱上**禁用**RetentionHold: 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - 现在, 重新运行托管文件夹助理:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **注意:** 如果邮箱小于 10 MB, 则托管文件夹助理将不会自动处理邮箱。 
  

