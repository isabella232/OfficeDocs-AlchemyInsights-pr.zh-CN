---
title: 需要有关电子邮件发送限制的帮助？
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 66ff82afd7b44ef5fd4943bfc794c2fa35bbfa9e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702353"
---
# <a name="need-help-with-email-sending-limits"></a>需要有关电子邮件发送限制的帮助？

下面是在服务中强制执行的**固有发送限制**。 有关这些限制的详细信息，请参阅[此处](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)。

- 为防止传递未经请求的批量邮件，我们将每用户**收件人速率限制应用于所有出站和内部邮件**。 在所有 SKU 中，此限制为每天**每天 10,000 个收件人**。  需要发送合法批量商业电子邮件的客户（例如，客户新闻稿）应使用专门提供这些服务的第三方提供商。
    - **注意**：达到收件人速率限制后，将无法从邮箱发送邮件，直到过去 24 小时内发送邮件的收件人数下降到限制之下。 在那之前，用户将不能发送邮件。
- 所有 SKU 均应用了邮件速率限制**每分钟 30 封邮件**。 这将决定用户在指定期间内可以从其 Exchange Online 帐户发送的邮件数。
- 在所有 SKU 中，一封电子邮件的 **“收件人”、“抄送”和“密件抄送”字段中允许的最大收件人数量**是 **1000 个收件人**。 若要自定义此限制，请转到[此处](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)。
