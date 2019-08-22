---
title: 美国/英国护照号码的 DLP 规则不起作用
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bc91af8be58d49204f84cd7d22f481348af3c013
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529909"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="c0cbf-102">有关 DLP-美国/英国护照号码的问题</span><span class="sxs-lookup"><span data-stu-id="c0cbf-102">Problems with DLP - US/UK Passport Numbers</span></span>

<span data-ttu-id="c0cbf-103">在 O365 中使用 DLP 敏感信息类型时, 您是否遇到**数据丢失防护 (DLP)** 无法处理包含**美国/英国护照号码**的内容的问题？</span><span class="sxs-lookup"><span data-stu-id="c0cbf-103">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK Passport Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="c0cbf-104">如果是这样, 请确保您的内容包含在评估时 DLP 策略要查找的内容所需的信息。</span><span class="sxs-lookup"><span data-stu-id="c0cbf-104">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="c0cbf-105">例如, 对于配置为可信度为 75% 的**美国/英国护照号码**策略, 将对以下项进行评估, 并且必须检测到规则才能触发</span><span class="sxs-lookup"><span data-stu-id="c0cbf-105">For example, for a **US/UK Passport Number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="c0cbf-106">**[格式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 九位数字</span><span class="sxs-lookup"><span data-stu-id="c0cbf-106">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="c0cbf-107">**[模式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 九个连续数字</span><span class="sxs-lookup"><span data-stu-id="c0cbf-107">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="c0cbf-108">**[校验和:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否, 没有校验和</span><span class="sxs-lookup"><span data-stu-id="c0cbf-108">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="c0cbf-109">**[定义:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** 如果 DLP 策略在300个字符的邻近度内检测到此类型的敏感信息, 则 DLP 策略 75% 确信它检测到这种类型的敏感信息:</span><span class="sxs-lookup"><span data-stu-id="c0cbf-109">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="c0cbf-110">函数 Func_usa_uk_passport 找到与该模式匹配的内容。</span><span class="sxs-lookup"><span data-stu-id="c0cbf-110">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="c0cbf-111">找到 Keyword_passport 中的一个关键字。</span><span class="sxs-lookup"><span data-stu-id="c0cbf-111">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="c0cbf-112">例如, 以下示例将触发**美国/英国护照号码**策略: 美国护照号码123456789</span><span class="sxs-lookup"><span data-stu-id="c0cbf-112">For example, the following sample would trigger for the **US/UK Passport Number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="c0cbf-113">若要详细了解为你的内容检测美国/英国护照号码时所需的信息, 请参阅本文中的以下部分:[敏感信息类型查找美国/英国护照号码的内容](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="c0cbf-113">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="c0cbf-114">使用不同的内置敏感信息类型, 请参阅以下文章, 了解其他类型所需的信息:[敏感信息类型查找的内容](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="c0cbf-114">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  