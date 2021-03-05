---
title: 查找对收件箱规则执行的事件
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
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464503"
---
# <a name="find-events-performed-on-inbox-rules"></a>查找在收件箱规则上执行的事件

创建、更改或删除收件箱规则时，事件将记录在审核日志。 下面将了解如何查看它们：

1. 转到 [Office 365 安全&合规中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。
1. 选择">审核日志搜索"。

    > [!NOTE]
    > 如果看到需要启用审核的通知，请继续，然后现在将其打开。 如果未启用此功能，搜索结果将无法从以前的日期提取数据。
1. 选择"活动"字段并查找 Exchange 邮箱活动，然后选择New-InboxRule创建收件箱规则Outlook Web App。 完成后，单击窗格外部以最小化"活动"窗格。
1. 指定日期范围，然后在"用户"字段中，选择要调查的用户的用户名。 一次可以选择多个用户。
1. 选择"搜索"。 活动显示在"结果"下。
1. 若要查看详细信息，请选择活动，然后选择"详细信息"。 在"参数"部分，你可以看到规则的名称、条件集以及规则将采取的操作。

若要了解更多信息，请参阅"搜索 Office 365 审核日志排查常见方案问题。