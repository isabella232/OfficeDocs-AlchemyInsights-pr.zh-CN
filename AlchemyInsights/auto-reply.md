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
ms.openlocfilehash: 1adc3c131daedb26d88710f4b4078b0622ad13c5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331521"
---
# <a name="to-configure-auto-reply-for-all-emails-sent-to-microsoft-365-group"></a>为发送到 Microsoft 365 组的所有电子邮件配置自动答复：

**使用租户管理员帐户连接到 EXO PowerShell 并使用以下命令**：

`Set-MailboxAutoReplyConfiguration -Identity groupmailbox -AutoReplyState Enabled -InternalMessage "Internal auto-reply message." -ExternalMessage "External auto-reply message`

**注意**：将 **groupmailbox** 更改为要在其上配置自动答复的组名称。

