---
title: 将电子邮件移动到存档邮箱
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974947"
---
# <a name="move-email-to-the-archive-mailbox"></a>将电子邮件移动到存档邮箱

如果您希望我们针对下面提到的设置运行自动检查，请选择此页面顶部的"后退"按钮"<"，然后输入将电子邮件移动到存档邮箱时遇到问题的用户的电子邮件地址。

1. 确认已 **启用存档** 邮箱。 如果没有，请使用本文 [中的步骤](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) 启用存档邮箱。

2. 若要将邮件自动存档到存档邮箱，必须将包含"移动到存档"操作的保留标记设置为自动应用于整个邮箱 (**默认) 标记**。 使用下面的步骤创建标记 [：Archive Default 标记](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)。

3. 接下来，将 **Archive** 标记添加到保留策略。 In the Exchange admin center， choose **Retention Policies** > add the Move to **Archive tag** to the policy > **Save**.

4. 现在 [，将保留策略](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) 分配给特定用户的邮箱。 相同的策略将应用于主 **邮箱和****存档** 邮箱。

可能需要强制托管文件夹助理 (MFA) 运行新设置，以及将新设置应用到用户邮箱。 连接到 [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) 时运行以下命令，为特定邮箱启动托管文件夹助理：
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

有关设置存档策略的信息，请参阅设置 [邮箱的存档和删除策略](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)。
  