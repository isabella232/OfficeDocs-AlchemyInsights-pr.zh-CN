---
title: 发件人未收到发送到 Microsoft 365 组的电子邮件
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/21/2020
ms.locfileid: "46846049"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>发件人未收到发送到 Microsoft 365 组的电子邮件

默认情况下，向 Microsoft 365 组发送电子邮件的发件人不会在其“收件箱”中收到该邮件的副本，即使发件人是该组的成员也是如此。

使用此 EXO PowerShell 命令使发件人可以收到他们发送给 Microsoft 365 组的每封电子邮件的副本：  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

若要立即为所有邮箱启用该设置，请执行以下操作：

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**注意** 对此设置的更改最多可能需要 1 个小时才会生效。