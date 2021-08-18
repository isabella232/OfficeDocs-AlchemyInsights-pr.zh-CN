---
title: 调查所有用户的活动
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332333"
---
# <a name="investigate-all-the-users-activities"></a>调查所有用户的活动

下面将对此进行说明：

1. 执行以下操作之一：
   - In the Microsoft 365 合规中心 at <https://compliance.microsoft.com> ， go to **Solutions** \> **Audit**. 或者，若要直接转到审核 **页面** ，请使用 <https://compliance.microsoft.com/auditlogsearch> 。
   - In the Microsoft 365 Defender portal at <https://security.microsoft.com> ， go to **Audit**. 或者，若要直接转到审核 **页面** ，请使用 <https://security.microsoft.com/auditlogsearch> 。

    **注意**：如果看到需要打开该功能的通知，请继续，然后打开它。 如果未启用此功能，搜索结果将无法从以前的日期提取数据。

2. 在"**审核****"页的**"搜索"选项卡上，配置以下设置：
   - **日期和时间范围**：在"开始"和"结束"框中 **选择日期** / **时间** 范围。
   - **活动**：如果你对特定活动感兴趣，请从列表中选择它;否则，默认值" **显示所有活动的结果"将** 返回所有活动。
   - **用户**：接受空白默认值以返回所有用户的结果，或输入一个或多个用户。

3. 完成后，单击"搜索 **"。** 活动显示在新的"审核搜索 **"页上** 。 你将看到 IP **地址、****用户****和活动名称**。

4. 若要下载结果，请选择"**导出** \> **下载所有结果"。**

5. 在结果中选择一个活动以打开详细信息飞出。

若要了解更多信息，请参阅 [搜索审核日志以调查常见的支持问题](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)。
