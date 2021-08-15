---
title: 确定审核日志中的收件箱规则活动
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e27c6433c65079af93f2a02a998b7179222336b0cae1149f4196f6fb6558ddac
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53976855"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>确定审核日志中的收件箱规则活动

您可以使用 审核日志 安全Microsoft 365合规性&中的搜索来查看收件箱规则事件 (创建、修改和删除收件箱规则) 。

1. 登录到合规性Microsoft 365[中心](https://protection.office.com/)。

2. 转到"**搜索**  >  **审核日志搜索"** 页。

3. 在"开始日期"和"结束日期 **"** 字段中 **选择日期** 范围。

4. 在 **Exchange活动**"下，验证"活动"字段是否设置为 **New-InboxRule Create/modify/enable/disable inbox rule**。

5. 单击"搜索"。

在结果中，选择审核记录。 在详细信息飞出中，单击 **"详细信息"。** 有关收件箱规则设置的信息显示在" **参数"** 字段中。

有关详细信息，请参阅确定 [用户是否创建了收件箱规则](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
