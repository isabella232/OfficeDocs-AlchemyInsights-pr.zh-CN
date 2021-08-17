---
title: 1385-Office-365-alert-policies
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: f5109445530ec4cc4988fb9c5d37145c45794ced6920607ce6df85c6497c25ec
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57891669"
---
# <a name="alert-policies"></a>警报策略

Microsoft 365包含默认[警报](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies)策略，这些策略可触发具有 Microsoft 365 企业版 或 Microsoft 365 美国政府版 E1/G1、E3/G3 或 E5/G5 订阅的组织发出警报。 因此，管理员可能会收到由管理员发送 Office365Alerts@microsoft.com 警报电子邮件通知，其中的主题行为"低严重性警报：警报 *策略的名称*"。 为常见活动触发警报时（例如，当用户：

- 创建转发电子邮件的收件箱规则。
- 为其邮箱分配权限。
- 在文件共享中共享或删除SharePoint文件。
- 创建电子数据展示搜索并导出搜索结果。

查看和操作警报：

1. 采取以下步骤之一：
   - In the Microsoft 365 合规中心 at <https://compliance.microsoft.com> ， go to **Alerts**. 或者，若要直接转到 **警报** 页面，请使用 <https://compliance.microsoft.com/compliancealerts> 。
   - In the Microsoft 365 Defender portal at <https://security.microsoft.com> ， go to **Incidents &** \> **alerts**. 或者，若要直接转到 **警报** 页面，请使用 <https://security.microsoft.com/alerts> 。
2. 单击警报以显示包含有关警报信息的飞出页。

你可以对警报采取操作，例如 [删除可疑的收件箱规则](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)。 或者，只需单击警报飞 **出页面上的** "解析"即可关闭警报。

有关配置和管理警报策略的信息，请参阅  [本文](https://docs.microsoft.com/microsoft-365/compliance/alert-policies)。

**重要** 提示：提醒来自 Microsoft 的电子邮件通知永远不会要求你执行以下操作：

- 提供密码
- 验证帐户的安全详细信息
- 重新验证你自己

如果您收到包含这些类型的请求的电子邮件，该邮件不是由 Microsoft 发送的，应视为欺诈邮件。 如果您收到包含这些类型的请求的邮件， [则向 Microsoft 报告该邮件](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)。
