---
title: 读取已删除事件的审核日志
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
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324723"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>读取已删除事件的审核日志

下面将对此进行说明：

1. 执行以下操作之一：
   - In the Microsoft 365 合规中心 at <https://compliance.microsoft.com> ， go to **Solutions** \> **Audit**. 或者，若要直接转到审核 **页面** ，请使用 <https://compliance.microsoft.com/auditlogsearch> 。
   - In the Microsoft 365 Defender portal at <https://security.microsoft.com> ， go to **Audit**. 或者，若要直接转到审核 **页面** ，请使用 <https://security.microsoft.com/auditlogsearch> 。

    **注意**：如果看到需要打开该功能的通知，请继续，然后打开它。 如果未启用此功能，搜索结果将无法从以前的日期提取数据。

2. 在"**审核****"页的**"搜索"选项卡上，配置以下设置：
   - **日期和时间范围**：在"开始"和"结束"框中 **选择日期** / **时间** 范围。
   - **活动****：Exchange邮箱活动，** 然后选择以下值：
     - **已从“已删除邮件”文件夹中删除邮件**
     - **已将邮件移动到“已删除邮件”文件夹**

       完成后，在窗格外单击以最小化" **活动"** 窗格。

   - **用户**：接受空白默认值以返回所有用户的结果，或输入一个或多个用户。

3. 完成后，单击"搜索 **"。** 活动显示在新的"审核搜索 **"页上** 。

4. 在结果中选择一个活动以打开详细信息飞出。 有关已删除项目的其他信息（如主题行和项目被删除时的位置）将显示在 **AffectedItems** 字段中。

   **注意**：无法还原使用"已删除邮件"功能审核日志项。 若要还原已删除的项目，请参阅恢复已删除的电子邮件[Outlook 网页版。](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11)

有关详细信息，请参阅搜索 [审核日志以调查常见的支持问题](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)。
