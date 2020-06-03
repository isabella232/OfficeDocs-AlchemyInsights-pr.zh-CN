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
# <a name="retention-policies-in-exchange-admin-center"></a>Exchange 管理中心中的保留策略

 **问题：** Exchange 管理中心中新创建或更新的保留策略不会应用于邮箱或项目不会移动到存档邮箱或将其删除。 
  
 **根本原因：**
  
- 这可能是因为**托管文件夹助理**尚未处理用户的邮箱。 托管文件夹助理每七天尝试处理一次基于云的组织中的每个邮箱。 如果您更改保留标记或向邮箱应用不同的保留策略，则可以等待托管文件夹帮助处理邮箱，也可以运行 Start-managedfolderassistant cmdlet 以启动托管文件夹助理来处理特定邮箱。 运行此 cmdlet 对于测试或排除保留策略或保留标记设置的故障很有用。 有关详细信息，请参阅[运行托管文件夹助理](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)。
    
  - **解决方案：** 运行以下命令以启动特定邮箱的托管文件夹助理：
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- 如果已在邮箱上启用**RetentionHold** ，也**enabled**可能出现此情况。 如果已将邮箱放在 RetentionHold 中，则邮箱中的保留策略将不会在该时间进行处理。 有关 RetentionHold 设置的详细 informaton，请参阅：[邮箱保留挂起](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)。
    
    **办法**
    
  - 检查[EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)中特定邮箱上的 RetentionHold 设置的状态：
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - 运行以下命令，在特定邮箱上**禁用**RetentionHold：
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - 现在，重新运行托管文件夹助理：
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **注意：** 如果邮箱小于 10 MB，则托管文件夹助理将不会自动处理邮箱。
 
有关 Exchange 管理中心中的保留策略的详细信息，请参阅：
- [保留标记和保留策略](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [将保留策略应用于邮箱](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [添加或删除保留标记](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [如何识别为邮箱设置的保留类型](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
