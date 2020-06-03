---
title: 将电子邮件移动到存档邮箱
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511030"
---
# <a name="move-email-to-the-archive-mailbox"></a>将电子邮件移动到存档邮箱

1. 确认已启用**存档邮箱**。 如果不是，请使用[本文](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)中的步骤启用存档邮箱。

2. 若要将邮件自动存档到存档邮箱，必须将包含 "**移动到存档**" 操作的保留标记设置为 "已**自动应用于整个邮箱（默认）" 标记**。 使用此处的步骤创建标记：[存档默认标记](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)。

3. 接下来，将**存档**标记添加到保留策略中。 在 Exchange 管理中心中，选择 "**保留策略**" > 将 "**移动到存档" 标记**添加到策略中 >**保存**。

4. 现在，[将保留策略分配](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)给特定用户的邮箱。 同一策略将同时应用于**主**邮箱和**存档**邮箱。

可能需要强制托管文件夹助理（MFA）运行并将新设置应用到用户的邮箱。 在[连接到 EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)时运行以下命令，以启动特定邮箱的托管文件夹助理：
  
启动-Start-managedfolderassistant-Identity<name of the mailbox>

有关设置存档策略的详细信息，请参阅[设置邮箱的存档和删除策略](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)。
  