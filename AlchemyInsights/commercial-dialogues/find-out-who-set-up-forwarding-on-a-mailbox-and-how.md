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
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988169"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>了解谁在邮箱上设置转发以及如何

如果对邮箱设置了外部转发，活动会作为 Set-Mailbox cmdlet 的一部分进行审核。 下面将了解如何在活动审核日志：

1. 转到安全Office 365[合规&中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。
1. 选择 **"搜索** >  **审核日志搜索"。**
    > [!NOTE]
    > 如果看到需要启用审核的通知，请继续，然后现在将其打开。 如果未启用此功能，搜索结果将无法从以前的日期提取数据。
1. 确保" **活动"** 字段设置为"显示默认 **活动** (活动的结果) 。 指定日期范围。 无需指定用户名。
1. 选择“**搜索**”。 这些活动出现在“**结果**”下。
1. 选择 **"筛选结果**"，然后在"活动筛选器"字段中输入 **"Set-mailbox"。**  这将返回所有 **Set-Mailbox** 活动。
1. 若要查看详细信息，请选择一个活动， **然后选择详细信息**。 在 **"** 参数"下，可以看到邮箱上设置的转发电子邮件地址。 **UserID** 表示在邮箱上设置外部转发的用户。
若要了解更多信息，请参阅[搜索Office 365 审核日志常见方案疑难解答](https://go.microsoft.com/fwlink/?linkid=2103944)。