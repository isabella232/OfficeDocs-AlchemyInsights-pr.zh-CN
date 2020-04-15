---
title: 设置用户邮箱的自动答复
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: e3cc01298c10fd3ba21327a7fb5cc5396d0ad74d
ms.sourcegitcommit: 23e5b94f1758bfe202008384e300b81816975375
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43506422"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a>设置用户邮箱的自动答复

**方法 1**

1. 登录 Office 365 门户。

2. 转到 **“用户”>“活动用户”**（或如果在共享邮箱上进行设置，则转到 **“组”>“共享邮箱”**）。

3. 选择具有 Microsoft Exchange 邮箱的用户。

4. 在右侧的弹出菜单上，转到 **“邮件设置”>“自动答复”**（如果是共享邮箱，只需在弹出菜单上单击“**自动答复**”）。

**方法 2**

1. 使用管理员凭据登录到 Office 365 管理门户。

2. 展开“**管理中心**”，然后单击“**Exchange**”。

3. 单击右上角的图片，单击“**其他用户**”，然后选择要更改的用户邮箱。

4. 在左侧，选择“**选项**”，单击“**组织电子邮件**”，然后单击“**自动答复**”。

**方法 3**

在 Exchange Online PowerShell 中运行以下 cmdlet：

PowerShellCopy

    Set-MailboxAutoReplyConfiguration

有关此 cmdlet 的详细信息，请参阅 [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration)。
