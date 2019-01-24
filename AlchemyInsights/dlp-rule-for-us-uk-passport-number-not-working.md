---
title: 美国的 DLP 规则 / 英国护照号码不起作用
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 716d1030d93ce006c36d7925fb132e974ae8feb4
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29459502"
---
<span data-ttu-id="56b5c-p101">您有未正常运行的内容包含**数据丢失防护 (DLP)** 问题**美国 / 英国护照号码**时使用 O365 中的 DLP 敏感信息类型？如果是这样，确保您的内容包含所需的信息的 DLP 策略查找的内容时对它求值。</span><span class="sxs-lookup"><span data-stu-id="56b5c-p101">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365? If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span> 
  
<span data-ttu-id="56b5c-104">例如，对于**美国 / 英国护照号码**配置的 75%的可信度级别的策略，以下计算和必须要触发的规则检测到</span><span class="sxs-lookup"><span data-stu-id="56b5c-104">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span> 
  
- <span data-ttu-id="56b5c-105">**[格式：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 九个数字</span><span class="sxs-lookup"><span data-stu-id="56b5c-105">**[Format:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span> 
    
- <span data-ttu-id="56b5c-106">**[模式：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 九个连续的数字</span><span class="sxs-lookup"><span data-stu-id="56b5c-106">**[Pattern:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span> 
    
- <span data-ttu-id="56b5c-107">**[校验和：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否，没有无校验和</span><span class="sxs-lookup"><span data-stu-id="56b5c-107">**[Checksum:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="56b5c-108">**[定义：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP 策略是相信它已检测到此类型的敏感信息的 75 %if、 内 300 个字符的邻近性：</span><span class="sxs-lookup"><span data-stu-id="56b5c-108">**[Definition:](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="56b5c-109">函数 Func_usa_uk_passport 找到与该模式匹配的内容。</span><span class="sxs-lookup"><span data-stu-id="56b5c-109">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>
    
  - <span data-ttu-id="56b5c-110">找到 Keyword_passport 中的一个关键字。</span><span class="sxs-lookup"><span data-stu-id="56b5c-110">A keyword from Keyword_passport is found.</span></span>
    
    <span data-ttu-id="56b5c-111">例如，下面的示例将触发的**美国 / 英国护照号码**策略： 美国护照号码 123456789</span><span class="sxs-lookup"><span data-stu-id="56b5c-111">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span> 
    
<span data-ttu-id="56b5c-112">上必需美国的详细信息 / 英国护照号码检测到了用于您的内容，请参阅本文中的以下部分：[什么敏感信息类型外观美国 / 英国护照号码](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="56b5c-112">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="56b5c-113">使用不同的内置敏感信息类型，请参阅以下文章，获取信息什么是需要其他类型：[查找什么敏感信息类型](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="56b5c-113">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

