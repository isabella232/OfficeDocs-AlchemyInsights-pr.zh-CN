---
title: 检索审核日志
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/16/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10964"
- "3100005"
ms.openlocfilehash: ac2e5eafbb92b234697c22f73cd565af9d7c3508
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329484"
---
# <a name="retrieve-the-audit-logs"></a>检索审核日志

首次打开审核日志时，它为空。 请搜索查看其中有什么内容。 以下是对所有活动进行常规搜索的方式：

1. 请按照以下步骤之一操作：
   - 在位于 <https://compliance.microsoft.com> 的 Microsoft 365 合规中心内，转到“**解决方案**”\>“**审核**”。 或使用 <https://compliance.microsoft.com/auditlogsearch> 直接转到“**审核**”页面。
   - 在位于 <https://security.microsoft.com> 的 Microsoft 365 Defender 门户中，转到“**审核**”。 或使用 <https://sip.security.microsoft.com/auditlogsearch> 直接转到“**审核**”页面。

2. 在“**审核**”页上，验证是否已选择“**搜索**”选项卡，然后配置以下设置：
   - **日期和时间范围**：在“**开始**”和“**结束**”框中选择日期/时间范围。
   - **活动**：验证是否已选择“**显示所有活动的结果**”。
   - **用户**：接受空白默认值以返回所有用户的结果，或输入一个或多个用户。

3. 完成后，单击“**搜索**”。 活动显示在新的“**审核搜索**”页上。

4. 在结果中，单击“**筛选结果**”并在活动筛选器框中键入 **Set-Mailbox**。

5. 在结果中选择审核记录。 在“**详细信息**”浮出控件中，单击“**更多信息**”以查看更多信息，例如客户端、执行操作的用户等。
