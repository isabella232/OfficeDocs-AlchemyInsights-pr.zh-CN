---
title: SSN 的 DLP 规则不起作用
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: d2d21fb5546d36990d69b76e3ceb72ce2edf3d80
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404407"
---
<span data-ttu-id="91727-102">在使用 Office 365 中的敏感信息类型时, 您是否遇到**数据丢失防护 (DLP)** 无法处理包含**社会保险号码 (SSN)** 的内容的问题？</span><span class="sxs-lookup"><span data-stu-id="91727-102">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Social Security Number (SSN)** when using a sensitive information type in Office 365?</span></span> <span data-ttu-id="91727-103">如果是这样, 请确保您的内容包含 DLP 策略所需的信息所需的信息。</span><span class="sxs-lookup"><span data-stu-id="91727-103">If so, make sure your content contains the needed information for what the DLP policy is looking.</span></span> 
  
<span data-ttu-id="91727-104">例如, 对于配置为可信度为 85% 的 SSN 策略, 将对以下项进行评估, 并且必须检测到规则才能触发:</span><span class="sxs-lookup"><span data-stu-id="91727-104">For example, for an SSN policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="91727-105">**[格式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 个数字, 可以是格式化或无格式的模式</span><span class="sxs-lookup"><span data-stu-id="91727-105">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 digits, which may be in a formatted or unformatted pattern</span></span> 
    
- <span data-ttu-id="91727-106">**[模式:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** 四个函数在四种不同的模式中查找 ssn:</span><span class="sxs-lookup"><span data-stu-id="91727-106">**[Pattern:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Four functions look for SSNs in four different patterns:</span></span> 
    
  - <span data-ttu-id="91727-107">Func_ssn 查找具有 2011 年以前使用短划线或空格格式化的强格式的 SSN（ddd-dd-dddd 或 ddd dd dddd）</span><span class="sxs-lookup"><span data-stu-id="91727-107">Func_ssn finds SSNs with pre-2011 strong formatting that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="91727-108">Func_unformatted_ssn 查找具有 2011 年以前未格式化为 9 个连续数字的强格式的 SSN (ddddddddd)</span><span class="sxs-lookup"><span data-stu-id="91727-108">Func_unformatted_ssn finds SSNs with pre-2011 strong formatting that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
  - <span data-ttu-id="91727-109">Func_randomized_formatted_ssn 查找 2011 年后使用短划线或空格（ddd-dd-dddd 或 ddd dd dddd）格式化的 SSN</span><span class="sxs-lookup"><span data-stu-id="91727-109">Func_randomized_formatted_ssn finds post-2011 SSNs that are formatted with dashes or spaces (ddd-dd-dddd OR ddd dd dddd)</span></span>
    
  - <span data-ttu-id="91727-110">Func_randomized_unformatted_ssn 查找 2011 年后未格式化为 9 个连续数字 (ddddddddd) 的 SSN</span><span class="sxs-lookup"><span data-stu-id="91727-110">Func_randomized_unformatted_ssn finds post-2011 SSNs that are unformatted as nine consecutive digits (ddddddddd)</span></span>
    
- <span data-ttu-id="91727-111">**[校验和:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** 否, 没有校验和</span><span class="sxs-lookup"><span data-stu-id="91727-111">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** No, there is no Checksum</span></span> 
    
- <span data-ttu-id="91727-112">**[定义:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** 如果 DLP 策略在300个字符的邻近度内检测到此类型的敏感信息, 则 DLP 策略 85% 确信它检测到这种类型的敏感信息:</span><span class="sxs-lookup"><span data-stu-id="91727-112">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span> 
    
  - <span data-ttu-id="91727-113">[函数 Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)找到与该模式匹配的内容。</span><span class="sxs-lookup"><span data-stu-id="91727-113">The [function Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) finds content that matches the pattern.</span></span> 
    
  - <span data-ttu-id="91727-114">找到 [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) 中的一个关键字。</span><span class="sxs-lookup"><span data-stu-id="91727-114">A keyword from [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) is found.</span></span> <span data-ttu-id="91727-115">关键字的示例包括:*社会保险、社会 security #、Soc Sec、SSN* 。</span><span class="sxs-lookup"><span data-stu-id="91727-115">Examples of keywords includes:  *Social Security, Social Security#, Soc Sec ,SSN*  .</span></span> <span data-ttu-id="91727-116">例如, 以下示例将触发 DLP SSN 策略: **SSN: 489-36-8350**</span><span class="sxs-lookup"><span data-stu-id="91727-116">For example, the following sample would trigger for the DLP SSN policy: **SSN: 489-36-8350**</span></span>
    
<span data-ttu-id="91727-117">若要详细了解为您的内容检测 ssn 所需的信息, 请参阅本文中的以下部分:[敏感信息类型查找的内容 ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span><span class="sxs-lookup"><span data-stu-id="91727-117">For more information on what is required for SSNs to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)</span></span>
  
<span data-ttu-id="91727-118">使用不同的内置敏感信息类型, 请参阅以下文章, 了解其他类型所需的信息:[敏感信息类型查找的内容](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="91727-118">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  

