---
title: 了解谁在邮箱上设置了转发，以及如何
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464374"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>了解谁在邮箱上设置了转发，以及如何

如果在邮箱上设置了外部转发，则活动作为 Set-Mailbox cmdlet 的一部分进行审核。 下面将了解如何在活动审核日志：

1. 转到 [Office 365 安全&合规中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。
1. 选择 **"搜索** >  **审核日志搜索"。**
    > [!NOTE]
    > 如果看到需要启用审核的通知，请继续，然后现在将其打开。 如果未启用此功能，搜索结果将无法从以前的日期提取数据。
1. 请确保将 **"活动** "字段设置为" **显示** 默认活动 (活动) 。 指定日期范围。 无需指定用户名。
1. 选择 **"搜索"。** 活动显示在"结果 **"下**。
1. 选择 **"筛选** 结果"，然后在"活动筛选器"字段中 **输入****Set-mailbox。** 这将返回 **所有 Set-Mailbox** 活动。
1. 若要查看详细信息，请选择一个活动，然后选择 **"详细信息"。** 在 **"** 参数"下，可以看到邮箱上设置的转发电子邮件地址。 **UserID** 表示在邮箱上设置外部转发的用户。
若要了解更多信息，请参阅["搜索 Office 365 审核日志排查常见方案。](https://go.microsoft.com/fwlink/?linkid=2103944)