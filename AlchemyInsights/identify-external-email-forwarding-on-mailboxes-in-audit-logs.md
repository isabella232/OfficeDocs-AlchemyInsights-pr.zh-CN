---
title: 在审核日志中标识邮箱的外部电子邮件转发
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331149"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>确定何时在邮箱上配置外部电子邮件转发

当Microsoft 365配置邮箱上的外部电子邮件转发时，活动会作为 **Set-Mailbox** cmdlet 的一部分进行审核。 可以使用搜索功能查看审核日志活动。 下面将说明如何执行。

1. 采取以下步骤之一：
   - In the Microsoft 365 合规中心 at <https://compliance.microsoft.com> ， go to **Solutions** \> **Audit**. 或者，若要直接转到审核 **页面** ，请使用 <https://compliance.microsoft.com/auditlogsearch> 。
   - In the Microsoft 365 Defender portal at <https://security.microsoft.com> ， go to **Audit**. 或者，若要直接转到审核 **页面** ，请使用 <https://sip.security.microsoft.com/auditlogsearch> 。

2. 在" **审核** "页上，验证"搜索 **"** 选项卡是否被选中，然后配置以下设置：
   - 在"开始"和"结束 **"框中选择日期/****时间** 范围。
   - 验证"**活动"** 框 **是否包含"显示所有活动的结果"。**

3. 完成后，单击"搜索 **"。** 活动显示在新的"审核搜索 **"页上** 。

4. 在结果中，单击"**筛选结果"，** 在活动筛选器框中键入 **Set-Mailbox。**

5. 在结果中选择审核记录。 在"**详细信息"** 飞出中，单击 **"详细信息"。** 您需要查看每个审核记录的详细信息，以确定活动是否与电子邮件转发相关。

   - **ObjectId：** 已修改邮箱的别名值。
   - **参数** _：ForwardingSmtpAddress_ 指示目标电子邮件地址。
   - **UserId：** 在 **"ObjectId"** 字段中配置邮箱电子邮件转发的用户。

有关详细信息，请参阅确定 [谁为邮箱设置了电子邮件转发](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)。
