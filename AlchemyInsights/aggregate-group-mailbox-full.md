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
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a><span data-ttu-id="1d815-102">为发送到 Microsoft 365 组的电子邮件接收的 AggregateGroupMailbox 完整 NDR</span><span class="sxs-lookup"><span data-stu-id="1d815-102">AggregateGroupMailbox full NDR received for email sent to Microsoft 365 group</span></span>

<span data-ttu-id="1d815-103">使用以下 EXO 命令行管理程序命令创建 Exchange 传输规则，以静默方式删除发送到聚合组邮箱的电子邮件：</span><span class="sxs-lookup"><span data-stu-id="1d815-103">Use the following EXO Shell command to create an Exchange transport rule to silently drop emails sent to aggregate group mailbox:</span></span>

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> <span data-ttu-id="1d815-104">将 **-SentTo** 中的 SMTP 地址替换为租户中聚合组邮箱的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="1d815-104">Replace the SMTP address in **-SentTo** with SMTP address of aggregate group mailbox in your tenant.</span></span> <span data-ttu-id="1d815-105">可以从收到的 NDR 获取聚合组邮箱的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="1d815-105">You can get the SMTP address of aggregate group mailbox from the NDR received.</span></span>



