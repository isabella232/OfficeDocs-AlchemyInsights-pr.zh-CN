---
title: 邮箱接收限制的执行
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58829144"
---
# <a name="mailbox-receiving-limit-enforcement"></a>邮箱接收限制的执行

Microsoft 最近开始强制实施每小时 3600 封邮件的每个邮箱阈值。 有关详细信息，请参阅 [Exchange Online 限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits)。 Microsoft 365 邮箱如果在一小时内接收超过 3600 封邮件，则将在接下来的 60 分钟内受到限制。 

此外，还应用了发件人 - 收件人对 (SRP) 的限制，阻止 Microsoft 365 邮箱接收到来自特定发件人的邮件。 如果单个发件人每个滚动小时向某个特定收件人发送超过总阈值 33% 或 1200 封邮件，则 SRP 限制将会启动，而邮箱将不再接受该发件人的邮件。 请注意:

- 此限制适用于从其他租户、本地或 Internet 发件人接收的电子邮件。
- 在接下来的 60 分钟内，将阻止向邮箱发送的电子邮件。 
- 这些邮箱的发件人会收到一份未送达报告 (5.2.121 或 5.2.122)，说明该邮箱已经超过了最大送达阈值。 租户内 (同一租户内的邮件) 将继续传递。
- 应用 SRP 限制后，接收邮箱将继续接受来自其他发件人的邮件。

管理员可以通过访问名为“超过接收限制的邮箱”的 Exchange 管理中心的新报告和见解来监控当前的邮箱活动。 仅当租户有违规邮箱时才会出现见解，而报告总是出现在仪表板中，但除非租户有违规邮箱，否则则为空。

有关见解接收限制的详细信息，请参阅 [新版 EAC 中超过接收限制的邮箱见解](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)。

有关超出接收限制报告的详细信息，请参阅 [新 EAC 中超过接收限制的邮箱报告](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)。