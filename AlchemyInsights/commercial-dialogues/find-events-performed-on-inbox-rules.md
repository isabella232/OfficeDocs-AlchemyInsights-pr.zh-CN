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
ms.openlocfilehash: 14a5a18bc1422572db567c9533fefe5a7e0120afd64df4a64623038cc063ce93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058640"
---
# <a name="find-events-performed-on-inbox-rules"></a>查找在收件箱规则上执行的事件

创建、更改或删除收件箱规则时，事件将记录在审核日志。 下面将了解如何查看它们：

1. 转到安全Office 365[合规&中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。
1. 选择"搜索>审核日志搜索"。

    > [!NOTE]
    > 如果看到需要启用审核的通知，请继续，然后现在将其打开。 如果未启用此功能，搜索结果将无法从以前的日期提取数据。
1. 选择"活动"字段并Exchange邮箱活动，然后选择"New-InboxRule创建收件箱规则"Outlook Web App。 完成后，在窗格外单击以最小化"活动"窗格。
1. 指定日期范围，然后在"用户"字段中，选择要调查的用户的用户名。 一次可以选择多个用户。
1. 选择“搜索”。 这些活动出现在“结果”下。
1. 若要查看详细信息，请选择一个活动，然后选择"详细信息"。 在"参数"部分下，可以看到规则的名称、条件集以及规则将采取的操作。

若要了解更多信息，请参阅搜索Office 365 审核日志常见方案疑难解答。