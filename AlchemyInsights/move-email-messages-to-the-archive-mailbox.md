---
title: 将电子邮件移动到存档邮箱
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: fb5745b60d42e1f7d7bb9b7a336a51b62c2ff92a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762355"
---
# <a name="move-email-to-the-archive-mailbox"></a>将电子邮件移动到存档邮箱
 
1. 确认已启用**存档邮箱**。 如果不是, 请使用[本文](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)中的步骤启用存档邮箱。

2. 若要将邮件自动存档到存档邮箱, 必须将包含 "**移动到存档**" 操作的保留标记设置为 "已**自动应用于整个邮箱 (默认)" 标记**。 使用此处的步骤创建标记:[存档默认标记](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0)。
    
3. 接下来, 将**存档**标记添加到保留策略中。 在 Exchange 管理中心中, 选择 "**保留策略**" > 将 "**移动到存档" 标记**添加到策略中 >**保存**。 
    
4. 现在,[将保留策略分配](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)给特定用户的邮箱。 同一策略将同时应用于**主**邮箱和**存档**邮箱。 
    
可能需要强制托管文件夹助理 (MFA) 运行并将新设置应用到用户的邮箱。 在[连接到 EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)时运行以下命令, 以启动特定邮箱的托管文件夹助理: 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

有关设置存档策略的详细信息, 请参阅[设置邮箱的存档和删除策略](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)。
  

