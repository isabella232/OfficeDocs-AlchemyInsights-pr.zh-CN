---
title: 检索审核日志
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
ms.openlocfilehash: 88d28898923c1381c001c15445da90901b7e8761
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320433"
---
# <a name="retrieve-the-audit-logs"></a>检索审核日志

第一次打开审核日志时，它将为空。 请搜索查看其中有什么内容。 以下是对所有活动进行常规搜索的方式：

1. 执行以下操作之一：
   - In the Microsoft 365 合规中心 at <https://compliance.microsoft.com> ， go to **Solutions** \> **Audit**. 或者，若要直接转到审核 **页面** ，请使用 <https://compliance.microsoft.com/auditlogsearch> 。
   - In the Microsoft 365 Defender portal at <https://security.microsoft.com> ， go to **Audit**. 或者，若要直接转到审核 **页面** ，请使用 <https://security.microsoft.com/auditlogsearch> 。

2. 在"**审核****"页的**"搜索"选项卡上，配置以下设置：
   - **日期和时间范围**：在"开始"和"结束"框中 **选择日期** / **时间** 范围。
   - **活动**：验证 **是否选择了"显示所有活动** 的结果"。
   - **用户**：接受空白默认值以返回所有用户的结果，或输入一个或多个用户。

3. 完成后，单击"搜索 **"。** 活动显示在新的"审核搜索 **"页上** 。

4. 在结果中选择一个活动以打开详细信息飞出。 你将看到更多信息，如客户端、已执行的操作的用户等。

若要了解更多信息，请参阅 [搜索审核日志以调查常见的支持问题](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)。
