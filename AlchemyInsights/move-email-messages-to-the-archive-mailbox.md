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
ms.openlocfilehash: 2147c70f64087bf95fc4e39c193caeac3b2c5361
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660365"
---
在遇到存档项目复制到存档邮箱的问题。请确保已执行以下步骤：
  
1. 确认已启用**存档邮箱**。如果没有，请使用[本文](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)中的步骤为启用存档邮箱。 
    
2. 在 Exchange 管理中心中，选择**合规性管理**下的**保留标记**中，使用**移动到存档**操作包含所需的**保留时间**创建**保留标记**。
    
3. 在 Exchange 管理中心中，选择**保留策略**、 创建**保留策略**和将您**移动到存档**保留标记添加到该策略。 
    
4. 向特定用户的邮箱中[分配将保留策略](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)。将相同的策略将应用于**主要**和**存档**邮箱。 
    
现在，用户的邮箱应具有将项目移动到存档邮箱的存档策略。可能需要强制托管文件夹助理 (MFA) 运行，并将新设置应用于用户的邮箱。运行下面的命令时[连接到 EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)启动托管文件夹助理特定邮箱的： 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

要设置存档策略的详细信息，请参阅[Set up 邮箱的存档和删除策略](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)。
  

