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
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="dbcee-102">需要有关电子邮件发送限制的帮助？</span><span class="sxs-lookup"><span data-stu-id="dbcee-102">Need help with email sending limits?</span></span>

<span data-ttu-id="dbcee-103">下面是在服务中强制执行的**固有发送限制**。</span><span class="sxs-lookup"><span data-stu-id="dbcee-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="dbcee-104">有关这些限制的详细信息，请参阅[此处](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)。</span><span class="sxs-lookup"><span data-stu-id="dbcee-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="dbcee-105">为防止传递未经请求的批量邮件，我们将每用户**收件人速率限制应用于所有出站和内部邮件**。</span><span class="sxs-lookup"><span data-stu-id="dbcee-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="dbcee-106">在所有 SKU 中，此限制为每天**每天 10,000 个收件人**。</span><span class="sxs-lookup"><span data-stu-id="dbcee-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="dbcee-107">需要发送合法批量商业电子邮件的客户（例如，客户新闻稿）应使用专门提供这些服务的第三方提供商。</span><span class="sxs-lookup"><span data-stu-id="dbcee-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="dbcee-108">**注意**：达到收件人速率限制后，将无法从邮箱发送邮件，直到过去 24 小时内发送邮件的收件人数下降到限制之下。</span><span class="sxs-lookup"><span data-stu-id="dbcee-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="dbcee-109">在那之前，用户将不能发送邮件。</span><span class="sxs-lookup"><span data-stu-id="dbcee-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="dbcee-110">所有 SKU 均应用了邮件速率限制**每分钟 30 封邮件**。</span><span class="sxs-lookup"><span data-stu-id="dbcee-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="dbcee-111">这将决定用户在指定期间内可以从其 Exchange Online 帐户发送的邮件数。</span><span class="sxs-lookup"><span data-stu-id="dbcee-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="dbcee-112">在所有 SKU 中，一封电子邮件的 **“收件人”、“抄送”和“密件抄送”字段中允许的最大收件人数量**是 **1000 个收件人**。</span><span class="sxs-lookup"><span data-stu-id="dbcee-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="dbcee-113">若要自定义此限制，请转到[此处](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)。</span><span class="sxs-lookup"><span data-stu-id="dbcee-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
