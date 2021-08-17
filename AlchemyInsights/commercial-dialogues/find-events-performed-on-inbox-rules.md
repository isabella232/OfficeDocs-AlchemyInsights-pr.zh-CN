---
title: 查找在收件箱规则上执行的事件
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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313489"
---
# <a name="find-events-performed-on-inbox-rules"></a>查找在收件箱规则上执行的事件

创建、更改或删除收件箱规则时，事件将记录在审核日志。 下面将了解如何查看它们：

1. 执行以下操作之一：
   - In the Microsoft 365 合规中心 at <https://compliance.microsoft.com> ， go to **Solutions** \> **Audit**. 或者，若要直接转到审核 **页面** ，请使用 <https://compliance.microsoft.com/auditlogsearch> 。
   - In the Microsoft 365 Defender portal at <https://security.microsoft.com> ， go to **Audit**. 或者，若要直接转到审核 **页面** ，请使用 <https://security.microsoft.com/auditlogsearch> 。

    **注意**：如果看到需要启用审核的通知，请继续，并打开它。 如果未启用此功能，搜索结果将无法从以前的日期提取数据。
1. 选择"活动"字段并查找Exchange活动，然后选择"New-InboxRule创建收件箱规则"Outlook Web App。 完成后，在窗格外单击以最小化"活动"窗格。
1. 指定日期范围，然后在"用户"字段中，选择要调查的用户的用户名。 一次可以选择多个用户。
1. 选择“搜索”。 这些活动出现在“结果”下。
1. 若要查看详细信息，请选择一个活动，然后选择"详细信息"。 在"参数"部分下，可以看到规则的名称、条件集以及规则将采取的操作。

2. 在"**审核****"页的**"搜索"选项卡上，配置以下设置：
   - **日期和时间范围**：在"开始"和"结束"框中 **选择日期** / **时间** 范围。
   - **活动**：从 **"新建收件箱规则"中选择"创建收件箱Outlook Web App**

3. 完成后，单击"搜索 **"。** 活动显示在新的"审核搜索 **"页上** 。

4. 在结果中选择一个活动以打开详细信息飞出。 在 **"参数"** 部分下，可以看到规则的名称、条件集以及规则将采取的操作。

若要了解更多信息，请参阅 [搜索审核日志以调查常见的支持问题](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)。
