---
title: 信用卡号的 DLP 规则不起作用
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932433"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="002b1-102">包含信用卡号的 DLP 问题</span><span class="sxs-lookup"><span data-stu-id="002b1-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="002b1-103">**重要说明**：许多 SharePoint Online 和 OneDrive 客户对在后台运行的服务运行关键业务应用程序。</span><span class="sxs-lookup"><span data-stu-id="002b1-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="002b1-104">其中包括内容迁移、数据丢失防护（DLP）和备份解决方案。</span><span class="sxs-lookup"><span data-stu-id="002b1-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="002b1-105">在这些前所未有的时间内，我们将采取措施，以确保在远程工作方案中，SharePoint Online 和 OneDrive 服务对依赖于该服务的用户保持高可用性和可靠性。</span><span class="sxs-lookup"><span data-stu-id="002b1-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="002b1-106">为支持此目标，我们已在工作日白天营业时对后台应用（迁移、DLP 和备份解决方案）实施了更严格的限制限制。</span><span class="sxs-lookup"><span data-stu-id="002b1-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="002b1-107">在这些情况中，您应认为这些应用程序的吞吐量非常有限。</span><span class="sxs-lookup"><span data-stu-id="002b1-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="002b1-108">但是，在夜间和周末的时间内，服务将准备好处理来自后台应用程序的较大数量的请求。</span><span class="sxs-lookup"><span data-stu-id="002b1-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="002b1-109">**包含信用卡号的 DLP 问题**</span><span class="sxs-lookup"><span data-stu-id="002b1-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="002b1-110">在 O365 中使用 DLP 敏感信息类型时，您是否遇到**数据丢失防护（DLP）** 无法处理包含**信用卡号**的内容的问题？</span><span class="sxs-lookup"><span data-stu-id="002b1-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="002b1-111">如果是这样，请确保您的内容包含在评估时触发 DLP 策略所需的信息。</span><span class="sxs-lookup"><span data-stu-id="002b1-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="002b1-112">例如，对于配置为可信度为85% 的**信用卡策略**，将对以下项进行评估，并且必须检测到规则才能触发：</span><span class="sxs-lookup"><span data-stu-id="002b1-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="002b1-113">**[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 位数字，可以是格式化或无格式（dddddddddddddddd），并且必须通过 Luhn 测试。</span><span class="sxs-lookup"><span data-stu-id="002b1-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="002b1-114">**[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** 一种非常复杂且强大的模式，可检测到全球所有主要品牌的卡，包括签证、MasterCard、发现卡、JCB、美洲 Express、礼品卡和用餐卡。</span><span class="sxs-lookup"><span data-stu-id="002b1-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="002b1-115">**[校验和：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** 是，Luhn 校验和</span><span class="sxs-lookup"><span data-stu-id="002b1-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="002b1-116">**[定义：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** 如果 DLP 策略在300个字符的邻近度内检测到此类型的敏感信息，则 DLP 策略85% 确信它检测到这种类型的敏感信息：</span><span class="sxs-lookup"><span data-stu-id="002b1-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="002b1-117">函数 Func_credit_card 找到与该模式匹配的内容。</span><span class="sxs-lookup"><span data-stu-id="002b1-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="002b1-118">下列其中一项为真：</span><span class="sxs-lookup"><span data-stu-id="002b1-118">One of the following is true:</span></span>

  - <span data-ttu-id="002b1-119">找到 Keyword_cc_verification 中的一个关键字。</span><span class="sxs-lookup"><span data-stu-id="002b1-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="002b1-120">找到 Keyword_cc_name 中的关键字</span><span class="sxs-lookup"><span data-stu-id="002b1-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="002b1-121">函数 Func_expiration_date 找到正确日期格式的日期。</span><span class="sxs-lookup"><span data-stu-id="002b1-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="002b1-122">校验和传递</span><span class="sxs-lookup"><span data-stu-id="002b1-122">The checksum passes</span></span>

    <span data-ttu-id="002b1-123">例如，以下示例将触发 DLP 信用卡号策略：</span><span class="sxs-lookup"><span data-stu-id="002b1-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="002b1-124">签证： 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="002b1-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="002b1-125">过期：2/2009</span><span class="sxs-lookup"><span data-stu-id="002b1-125">Expires: 2/2009</span></span>

<span data-ttu-id="002b1-126">若要详细了解为您的内容检测**信用卡号**需要什么，请参阅本文中的以下部分：[有关信用卡号的敏感信息类型的外观](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="002b1-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="002b1-127">使用不同的内置敏感信息类型，请参阅以下文章，了解其他类型所需的信息：[敏感信息类型查找的内容](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="002b1-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  