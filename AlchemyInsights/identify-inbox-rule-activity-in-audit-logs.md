---
title: 确定审核日志中的收件箱规则活动
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1201a625948743cacfaa58410abeb4108ed2eb56
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539127"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>确定审核日志中的收件箱规则活动

可以在 "Office 365 安全 & 合规中心" 中使用审核日志搜索, 以查看收件箱规则事件 (创建、修改和删除收件箱规则)。

1. 登录到[Office 365 安全 & 合规中心](https://protection.office.com/)。

2. 转到 "**搜索** > **审核日志搜索**" 页。

3. 在 "**开始日期**" 和 "**结束日期**" 字段中选择日期范围。

4. 在 " **Exchange 邮箱活动**" 下, 验证 "**活动**" 字段是否设置为**new-inboxrule "创建/修改/启用/禁用收件箱规则"**。

5. 单击"搜索"。

在结果中, 选择一个审核记录。 在 "详细信息" 浮出控件中, 单击 "**详细信息**"。 有关收件箱规则设置的信息将显示在 "**参数**" 字段中。

有关详细信息, 请参阅[确定用户是否已创建收件箱规则](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
