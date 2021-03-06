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
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>为发送到 Microsoft 365 组的所有电子邮件配置自动答复：

**使用租户管理员帐户连接到 EXO PowerShell 并使用以下命令**：

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

> [!NOTE]
> 将 **邮件发送** 更改为要用于配置自动答复的组名称。

