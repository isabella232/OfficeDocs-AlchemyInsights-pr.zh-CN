---
title: 了解谁在邮箱上设置转发以及如何
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: d6be4331967ed9ae362f5da85856b03cfa40b319
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317798"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>了解谁在邮箱上设置转发以及如何

如果对邮箱设置了外部转发，活动会作为 **Set-Mailbox** cmdlet 的一部分进行审核。 下面将说明如何查找活动审核日志：

1. 执行以下操作之一：
   - In the Microsoft 365 合规中心 at <https://compliance.microsoft.com> ， go to **Solutions** \> **Audit**. 或者，若要直接转到审核 **页面** ，请使用 <https://compliance.microsoft.com/auditlogsearch> 。
   - In the Microsoft 365 Defender portal at <https://security.microsoft.com> ， go to **Audit**. 或者，若要直接转到审核 **页面** ，请使用 <https://security.microsoft.com/auditlogsearch> 。

   **注意**：如果看到需要启用审核的通知，请继续，并打开它。 如果未启用此功能，搜索结果将无法从以前的日期提取数据。

2. 在" **审核** "页上，验证"搜索 **"** 选项卡是否被选中，然后配置以下设置：
   - 在"开始"和"结束 **"框中选择日期/****时间** 范围。
   - 验证"**活动"** 框 **是否包含"显示所有活动的结果"。**

3. 完成后，单击"搜索 **"。** 活动显示在新的"审核搜索 **"页上** 。

4. 在结果中，单击 **"活动** "列以对结果进行排序，然后查找 **"Set-Mailbox"** 条目。

5. 在结果中选择一个活动以打开详细信息飞出。 您需要查看每个审核记录的详细信息，以确定活动是否与电子邮件转发相关：
   - **ObjectId：** 已修改邮箱的别名值。
   - **参数** _：ForwardingSmtpAddress_ 指示目标电子邮件地址。
   - **UserId：** 在 **"ObjectId"** 字段中配置邮箱电子邮件转发的用户。

有关详细信息，请参阅确定 [谁为邮箱设置了电子邮件转发](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)。
