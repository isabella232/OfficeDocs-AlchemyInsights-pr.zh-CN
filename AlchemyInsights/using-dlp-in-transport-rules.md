---
title: 在传输规则中使用 DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827206"
---
# <a name="using-dlp-in-transport-rules"></a>在传输规则中使用 DLP

若要将数据丢失防护 (DLP) 集成到现有传输中，请在传输规则设置中使用条件“**如果邮件包含...敏感信息**”。

**有关详细信息，请参阅：**

- 在传输规则中集成 DLP 敏感信息类型：[集成敏感信息规则](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules)。

你也可以使用规则上的“测试模式”来测试规则（使用或不使用策略测试）。  创建规则后，应等待 30 分钟，然后再进行测试。

- 请参阅[测试邮件流/传输规则](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**注意**：如果你尝试使用 EAC 中的传输规则实施新的 DLP 策略，请改为使用 [安全与合规中心内的 DLP 策略](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide)。
