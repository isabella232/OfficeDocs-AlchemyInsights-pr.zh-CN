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
ms.openlocfilehash: 5b58803719df700290f495cb2d2d6742f072420a2a1d393534ca165bb5a14fbb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017122"
---
# <a name="find-the-ip-address-in-audit-log"></a>在"地址"中审核日志

1. 与用户或管理员执行的活动对应的 IP 地址显示在审核日志中。 还会记录客户端信息。 下面是如何标识 IP 地址的：

1. 转到安全Office 365[合规&中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。
1. 选择 **"搜索**  >  **[审核日志搜索"。](https://go.microsoft.com/fwlink/?linkid=2103759)**
    > [!NOTE]
    > 如果看到需要启用审核的通知，请继续，然后现在将其打开。 如果未启用此功能，搜索结果将无法拉取以前日期的数据。
1. 如果你对特定活动感兴趣，请从"活动" **列表中选择它;** 否则，默认情况下，将为所选用户返回所有活动。 请注意，某些活动可能无法从"活动 **"菜单中选择**;但是，如果选择默认设置"显示所有活动的结果"，将返回 (审核) 。
1. 指定日期范围，在"用户" **字段中，** 选择要调查的用户的用户名。
1. 选择“**搜索**”。 这些活动出现在“**结果**”下。 你可以看到每个活动的 IP 地址。
1. 若要查看详细信息，请选择一个活动， **然后选择详细信息**。

若要了解更多信息，请参阅搜索Office 365 审核日志[常见方案疑难解答](https://go.microsoft.com/fwlink/?linkid=2103944)。