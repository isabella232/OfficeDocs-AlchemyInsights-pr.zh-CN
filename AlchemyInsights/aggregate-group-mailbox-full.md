---
title: 为发送到 Microsoft 365 组的电子邮件接收的 AggregateGroupMailbox 完整 NDR
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
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2020
ms.locfileid: "49715665"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>为发送到 Microsoft 365 组的电子邮件接收的 AggregateGroupMailbox 完整 NDR

使用以下 EXO 命令行管理程序命令创建 Exchange 传输规则，以静默方式删除发送到聚合组邮箱的电子邮件：

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> 将 **-SentTo** 中的 SMTP 地址替换为租户中聚合组邮箱的 SMTP 地址。 可以从收到的 NDR 获取聚合组邮箱的 SMTP 地址。



