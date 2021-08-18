---
title: AggregateGroupMailbox 接收的发送到组的电子邮件的完整 NDR Microsoft 365 NDR
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: ace8e256e3771f82512abcb9e20b832381eedf80
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315900"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox 接收的发送到组的电子邮件的完整 NDR Microsoft 365 NDR

使用以下 EXO 命令行管理程序命令创建Exchange自动删除发送到聚合组邮箱的电子邮件：

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

**注意**：将 **-SentTo** 中的 SMTP 地址替换为租户中聚合组邮箱的 SMTP 地址。 可以从收到的 NDR 获取聚合组邮箱的 SMTP 地址。



