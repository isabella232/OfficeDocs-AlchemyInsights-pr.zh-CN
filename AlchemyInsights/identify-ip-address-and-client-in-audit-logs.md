---
title: 在审核日志中标识 IP 地址和客户端
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: fcad71bcc5ea6036bc8fa25a9be38caabc4d0889ee01ea86e23065333d5fce0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014890"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>在审核日志中标识 IP 地址和客户端

与用户或管理员Microsoft 365活动的 IP 地址显示在审核日志中。 还会记录客户端信息。 下面是标识此信息的步骤

1. 登录到合规性Microsoft 365[中心](https://protection.office.com/)。

2. 转到"**搜索**  >  **审核日志搜索"** 页。

   如果你对特定活动感兴趣，请从" **活动"列表中选择** 它。 如果不是，将返回所选用户的所有活动 (默认设置) 。

   **注意**：某些活动在"活动"菜单中 **可能** 不可用;但是，如果选择默认设置"显示所有活动的结果"，将返回 (审核) 。

3. 在"用户"**字段中指定** 用户名，为活动选择适当的日期范围，然后单击"搜索 **"。**

在结果中，您可以在结果窗格中看到该活动的 IP 地址。 Select the audit record to see detailed information in the **Details** flyout (for example， Client， User that performed action， etc.) .

有关详细信息，请参阅查找用于访问遭到入侵的帐户的计算机的 [IP 地址](/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)。
