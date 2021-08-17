---
title: 在"地址"中审核日志
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
ms.openlocfilehash: 258e92368b8a33e8ea807f0cb9af90132c86ed5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58303567"
---
# <a name="find-the-ip-address-in-audit-log"></a>在"地址"中审核日志

与用户或管理员执行的活动对应的 IP 地址显示在审核日志中。 还会记录客户端信息。 下面是如何标识 IP 地址的：

1. 执行以下操作之一：
   - In the Microsoft 365 合规中心 at <https://compliance.microsoft.com> ， go to **Solutions** \> **Audit**. 或者，若要直接转到审核 **页面** ，请使用 <https://compliance.microsoft.com/auditlogsearch> 。
   - In the Microsoft 365 Defender portal at <https://security.microsoft.com> ， go to **Audit**. 或者，若要直接转到审核 **页面** ，请使用 <https://security.microsoft.com/auditlogsearch> 。

    **注意**：如果看到需要启用审核的通知，请继续，并打开它。 如果未启用此功能，搜索结果将无法从以前的日期提取数据。

2. 在" **审核** "页上，验证"搜索 **"** 选项卡是否被选中，然后配置以下设置：
   - **日期和时间范围**：在"开始"和"结束"框中 **选择日期** / **时间** 范围。
   - **活动**：如果你对特定活动感兴趣，请从列表中选择它;否则，默认值" **显示所有活动的结果"** 将返回所有活动。 请注意，某些活动可能无法选择;但是，如果选择"显示所有活动的结果"，将返回 **这些** 审核项目。
   - **用户**：接受空白默认值以返回所有用户的结果，或输入一个或多个用户。

3. 完成后，单击"搜索 **"。** 活动显示在新的"审核搜索 **"页上** 。

4. 在结果中，单击"**筛选结果"，** 在活动筛选器框中键入 **Set-Mailbox。**

5. 在结果中选择审核记录以打开" **详细信息"** 飞出。

有关详细信息，请参阅搜索 [审核日志以调查常见的支持问题](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)。
