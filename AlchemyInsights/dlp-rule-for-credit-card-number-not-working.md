---
title: DLP 规则信用卡号不起作用
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919070"
---
<span data-ttu-id="7d169-p101">您是否有问题**数据丢失防护 (DLP)** 时使用 O365 中的 DLP 敏感信息类型包含**信用卡号**的内容不起作用？如果是这样，请确保您的内容包含所需的信息以触发 DLP 策略时对它求值。例如，对于配置了 85%可信度**信用卡策略**，以下计算和必须要触发的规则检测到：</span><span class="sxs-lookup"><span data-stu-id="7d169-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated. For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span> 
  
- <span data-ttu-id="7d169-105">**[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 位数字格式化或无格式 (dddddddddddddddd)，必须将传递 Luhn 测试。</span><span class="sxs-lookup"><span data-stu-id="7d169-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span> 
    
- <span data-ttu-id="7d169-106">**[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** 检测卡全球，包括 Visa、 Mastercard、 发现卡片、 JCB、 美国运通、 礼品卡和进餐卡的所有主要品牌从非常复杂和可靠的图案。</span><span class="sxs-lookup"><span data-stu-id="7d169-106">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span> 
    
- <span data-ttu-id="7d169-107">**[校验和：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** 是、 Luhn 校验和</span><span class="sxs-lookup"><span data-stu-id="7d169-107">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span> 
    
- <span data-ttu-id="7d169-108">**[定义：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP 策略是 85%相信它已检测到此类型的敏感信息 if、 内 300 个字符的邻近性：</span><span class="sxs-lookup"><span data-stu-id="7d169-108">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="7d169-109">函数 Func_credit_card 找到与该模式匹配的内容。</span><span class="sxs-lookup"><span data-stu-id="7d169-109">The function Func_credit_card finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="7d169-110">下列其中一项为真：</span><span class="sxs-lookup"><span data-stu-id="7d169-110">One of the following is true:</span></span> 
    
  - <span data-ttu-id="7d169-111">找到 Keyword_cc_verification 中的一个关键字。</span><span class="sxs-lookup"><span data-stu-id="7d169-111">A keyword from Keyword_cc_verification is found.</span></span>
    
  - <span data-ttu-id="7d169-112">找到从 Keyword_cc_name 关键字</span><span class="sxs-lookup"><span data-stu-id="7d169-112">A keyword from Keyword_cc_name is found</span></span>
    
  - <span data-ttu-id="7d169-113">函数 Func_expiration_date 找到正确日期格式的日期。</span><span class="sxs-lookup"><span data-stu-id="7d169-113">The function Func_expiration_date finds a date in the right date format.</span></span>
    
  - <span data-ttu-id="7d169-114">校验和传递</span><span class="sxs-lookup"><span data-stu-id="7d169-114">The checksum passes</span></span>
    
    <span data-ttu-id="7d169-115">例如，下面的示例将触发 DLP 信用卡号策略：</span><span class="sxs-lookup"><span data-stu-id="7d169-115">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>
    
  - <span data-ttu-id="7d169-116">Visa: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="7d169-116">Visa: 4485 3647 3952 7352</span></span> 
    
  - <span data-ttu-id="7d169-117">过期： 2/2009</span><span class="sxs-lookup"><span data-stu-id="7d169-117">Expires: 2/2009</span></span>
    
<span data-ttu-id="7d169-118">什么是**信用卡号**检测到了用于您的内容所需的详细信息，请参阅本文中的以下部分：[什么敏感信息类型查找信用卡 #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span><span class="sxs-lookup"><span data-stu-id="7d169-118">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="7d169-119">使用不同的内置敏感信息类型，请参阅以下文章，获取信息什么是需要其他类型：[查找什么敏感信息类型](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="7d169-119">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

