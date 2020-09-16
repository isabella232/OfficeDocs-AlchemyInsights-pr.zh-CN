---
title: 发件人未收到发送到 Microsoft 365 组的电子邮件
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b8091305d55408f51cf369506acc7bfac59defb5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751305"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="bd840-102">发件人未收到发送到 Microsoft 365 组的电子邮件</span><span class="sxs-lookup"><span data-stu-id="bd840-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="bd840-103">默认情况下，向 Microsoft 365 组发送电子邮件的发件人不会在其“收件箱”中收到该邮件的副本，即使发件人是该组的成员也是如此。</span><span class="sxs-lookup"><span data-stu-id="bd840-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="bd840-104">使用此 EXO PowerShell 命令使发件人可以收到他们发送给 Microsoft 365 组的每封电子邮件的副本：</span><span class="sxs-lookup"><span data-stu-id="bd840-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="bd840-105">若要立即为所有邮箱启用该设置，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="bd840-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="bd840-106">**注意** 对此设置的更改最多可能需要 1 个小时才会生效。</span><span class="sxs-lookup"><span data-stu-id="bd840-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>