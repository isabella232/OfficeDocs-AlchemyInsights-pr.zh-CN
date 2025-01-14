---
title: 确定审核日志中的收件箱规则活动
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331113"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>确定审核日志中的收件箱规则活动

您可以使用邮件审核日志搜索来Microsoft 365 合规中心收件箱规则事件， (、修改和删除收件箱规则) 。

1. 采取以下步骤之一：
   - In the Microsoft 365 合规中心 at <https://compliance.microsoft.com> ， go to **Solutions** \> **Audit**. 或者，若要直接转到审核 **页面** ，请使用 <https://compliance.microsoft.com/auditlogsearch> 。
   - 在 Microsoft 365 Defender门户中 <https://security.microsoft.com> ，转到审核。 或者，若要直接转到审核 **页面** ，请使用 <https://security.microsoft.com/auditlogsearch> 。

2. 在"**审核****"页的**"搜索"选项卡上，配置以下设置：
   - **日期和时间范围**：在"开始"和"结束"框中 **选择日期** / **时间** 范围。
   - **活动**：选择以下一个或多个值：
     - **New-InboxRule 从收件箱创建收件箱Outlook Web App**
     - **Set-InboxRule 修改来自 Outlook Web App 的规则**。
     - **从客户端更新Outlook规则**

3. 完成后，单击"搜索 **"。** 活动显示在新的"审核搜索 **"页上** 。

4. 在结果中选择一个活动以打开详细信息飞出。 有关收件箱规则设置的信息显示在" **参数"** 字段中。

有关详细信息，请参阅确定 [用户是否创建了收件箱规则](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)。
