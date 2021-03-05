---
title: 在邮件中查找 IP 审核日志
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
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464504"
---
# <a name="find-the-ip-address-in-audit-log"></a>在邮件中查找 IP 审核日志

1. 与用户或管理员执行的活动对应的 IP 地址显示在审核日志中。 还会记录客户端信息。 下面是如何标识 IP 地址的：

1. 转到 [Office 365 安全&合规中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。
1. 选择 **"搜索**  >  **[审核日志搜索"。](https://go.microsoft.com/fwlink/?linkid=2103759)**
    > [!NOTE]
    > 如果看到需要启用审核的通知，请继续，然后现在将其打开。 如果未启用此功能，搜索结果将无法从以前的日期拉取数据。
1. 如果您对特定活动感兴趣，请从"活动" **列表中选择它;** 否则，默认情况下，将为所选用户返回所有活动。 请注意，某些活动可能无法从"活动"菜单中 **选择**;但是，如果在默认设置下选中"显示所有活动的结果"， (将返回) 。
1. 指定日期范围，在"用户" **字段中，** 选择要调查的用户的用户名。
1. 选择 **"搜索"。** 活动显示在"结果 **"下**。 你可以看到每个活动的 IP 地址。
1. 若要查看详细信息，请选择一个活动，然后选择 **"详细信息"。**

若要了解更多信息，请参阅"[搜索 Office 365 审核日志排查常见方案。](https://go.microsoft.com/fwlink/?linkid=2103944)