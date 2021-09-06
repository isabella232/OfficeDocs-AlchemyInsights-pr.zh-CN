---
title: 需要有关电子邮件发送限制的帮助？
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
- "9002938"
- "5630"
ms.openlocfilehash: b55654f56ab405c93934fd1a0917f50c053b09466e877e1255adbd28db83d93f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097476"
---
# <a name="need-help-with-email-sending-limits"></a>需要有关电子邮件发送限制的帮助？

下面是在服务中强制执行的 **固有发送限制**。 有关这些限制的详细信息，请参阅[此处](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)。

- 为防止传递未经请求的批量邮件，我们将每用户 **收件人速率限制应用于所有出站和内部邮件**。 在所有 SKU 中，此限制为每天 **每天 10,000 个收件人**。  需要发送合法批量商业电子邮件的客户（例如，客户新闻稿）应使用专门提供这些服务的第三方提供商。
    - **注意**：一旦达到收件人速率限制，将无法从邮箱发送邮件，直至发送邮件的收件人数在过去 24 小时内下降到限制之下。在那之前，用户将无法发送邮件。
- 所有 SKU 均应用了邮件速率限制 **每分钟 30 封邮件**。 这将决定用户在指定期间内可以从其 Exchange Online 帐户发送的邮件数。
- 在所有 SKU 中，单封电子邮件的 **“收件人”、“抄送”、“密件抄送”中允许的最大收件人数** 是 **1000 名收件人**。若要自定义此限制，请转到 [此处](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)。
