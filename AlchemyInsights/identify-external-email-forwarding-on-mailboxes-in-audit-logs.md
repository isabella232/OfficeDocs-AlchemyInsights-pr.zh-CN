---
title: 确定审核日志中邮箱的外部电子邮件转发
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7defd0902e8c8bebae9c7bfee72c3199cbc1909f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539091"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>确定何时在邮箱上配置了外部电子邮件转发

当 Office 365 用户在邮箱上配置外部电子邮件转发时, 该活动将作为**设置邮箱**cmdlet 的一部分进行审核。 您可以使用安全 & 合规性中心中的 "审核日志搜索" 查看活动。

1. 登录到[Office 365 安全 & 合规中心](https://protection.office.com/)。

2. 转到 "**搜索** > **审核日志搜索**" 页。

3. 在 "**开始日期**" 和 "**结束日期**" 字段中选择日期范围。 无需指定用户名。 验证 "**活动**" 字段是否设置为**显示所有活动的结果**。

4. 单击"搜索"。

在结果中, 单击 "活动筛选器" 框中的 "**筛选结果**并键入 '**设置 '-邮箱**"。 在结果中选择一个审核记录。 在 "**详细**信息" 浮出控件中, 单击 "**详细信息**"。 您必须查看每个审核记录的详细信息, 以确定该活动是否与电子邮件转发相关。

- **ObjectId**: 已修改的邮箱的别名值。

- **参数**: _ForwardingSmtpAddress_表示目标电子邮件地址。

- **UserId**: 在**ObjectId**字段中的邮箱上配置电子邮件转发的用户。

有关详细信息, 请参阅[确定为邮箱设置电子邮件转发](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)。
