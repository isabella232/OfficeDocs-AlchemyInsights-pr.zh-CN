---
title: 为发送到 Microsoft 365 组的所有电子邮件配置自动答复：
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8586"
- "9003200"
ms.openlocfilehash: c3c1d4e6b16b54d92771d7bdecdc9cb12bbf888c
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430712"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a><span data-ttu-id="b5b83-102">为发送到 Microsoft 365 组的所有电子邮件配置自动答复：</span><span class="sxs-lookup"><span data-stu-id="b5b83-102">To configure auto reply for all emails sent to Microsoft 365 group:</span></span>

<span data-ttu-id="b5b83-103">**使用租户管理员帐户连接到 EXO PowerShell 并使用以下命令**：</span><span class="sxs-lookup"><span data-stu-id="b5b83-103">**Connect to EXO PowerShell using tenant admin account and use following command**:</span></span>

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

> [!NOTE]
> <span data-ttu-id="b5b83-104">将 **邮件发送** 更改为要用于配置自动答复的组名称。</span><span class="sxs-lookup"><span data-stu-id="b5b83-104">Change **groupmailbox** to a group name that you want to configure auto reply on.</span></span>

