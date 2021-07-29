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
ms.openlocfilehash: b7146b2b09b6ac1e33b192dcbcbfb72ea2593313
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630239"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>确定何时在邮箱上配置外部电子邮件转发

当Microsoft 365配置邮箱上的外部电子邮件转发时，活动会作为 **Set-Mailbox** cmdlet 的一部分进行审核。 您可以在安全与合规中心审核日志搜索&活动。

1. 登录到合规性Microsoft 365[中心](https://protection.office.com/)。

2. 转到"**搜索**  >  **审核日志搜索"** 页。

3. 在"开始日期"和"结束日期 **"** 字段中 **选择日期** 范围。 无需指定用户名。 验证 **"活动**"字段是否设置为 **"显示所有活动的结果"。**

4. 单击"搜索"。

在结果中，单击"**筛选结果"，** 在活动筛选器框中键入 **Set-Mailbox。** 在结果中选择审核记录。 在"**详细信息"** 飞出中，单击 **"详细信息"。** 您必须查看每个审核记录的详细信息，以确定活动是否与电子邮件转发相关。

- **ObjectId：** 已修改邮箱的别名值。

- **参数** _：ForwardingSmtpAddress_ 指示目标电子邮件地址。

- **UserId：** 在 **"ObjectId"** 字段中配置邮箱电子邮件转发的用户。

有关详细信息，请参阅确定 [谁为邮箱设置了电子邮件转发](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)。
