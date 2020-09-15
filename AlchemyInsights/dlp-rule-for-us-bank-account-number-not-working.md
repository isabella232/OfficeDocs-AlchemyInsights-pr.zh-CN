---
title: 适用于美国银行帐户编号的 DLP 规则不起作用
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679286"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a><span data-ttu-id="fded6-102">包含美国银行帐户号的 DLP 问题</span><span class="sxs-lookup"><span data-stu-id="fded6-102">DLP issues with US bank account numbers</span></span>

<span data-ttu-id="fded6-103">**重要信息：** 在这段前所未有的时期，我们正在采取措施确保 SharePoint Online 和 OneDrive 服务高度可用，请访问 [SharePoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)，获取详细信息。</span><span class="sxs-lookup"><span data-stu-id="fded6-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="fded6-104">**包含美国银行帐户号的 DLP 问题**</span><span class="sxs-lookup"><span data-stu-id="fded6-104">**DLP issues with US bank account numbers**</span></span>

<span data-ttu-id="fded6-105">您是否遇到 \*\*数据丢失防护问题 (dlp) \*\* 在 O365 中使用 DLP 敏感信息类型时，不能处理包含 **美国银行帐号** 的内容？</span><span class="sxs-lookup"><span data-stu-id="fded6-105">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US Bank Account Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="fded6-106">如果是这样，请确保您的内容包含在评估时 DLP 策略要查找的内容所需的信息。</span><span class="sxs-lookup"><span data-stu-id="fded6-106">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="fded6-107">例如，对于配置为可信度为85% 的 **美国银行帐户号** 策略，将对其进行评估，并且必须检测到规则才能触发以下条件：</span><span class="sxs-lookup"><span data-stu-id="fded6-107">For example, for a **US Bank Account Number** policy configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="fded6-108">**[格式：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 位</span><span class="sxs-lookup"><span data-stu-id="fded6-108">**[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 digits</span></span>

- <span data-ttu-id="fded6-109">**[Pattern：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 连续数字。</span><span class="sxs-lookup"><span data-stu-id="fded6-109">**[Pattern:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 consecutive digits.</span></span>

- <span data-ttu-id="fded6-110">**[校验和：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** 否，没有校验和</span><span class="sxs-lookup"><span data-stu-id="fded6-110">**[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="fded6-111">**[定义：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** 如果 DLP 策略在300个字符的邻近度内检测到此类型的敏感信息，则 DLP 策略75% 确信它检测到这种类型的敏感信息：</span><span class="sxs-lookup"><span data-stu-id="fded6-111">**[Definition:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="fded6-112">正则表达式 Regex_usa_bank_account_number 找到与该模式匹配的内容</span><span class="sxs-lookup"><span data-stu-id="fded6-112">The regular expression Regex_usa_bank_account_number finds content that matches the pattern</span></span>

  - <span data-ttu-id="fded6-113">找到 Keyword_usa_Bank_Account 中的一个关键字。</span><span class="sxs-lookup"><span data-stu-id="fded6-113">A keyword from Keyword_usa_Bank_Account is found.</span></span>

    <span data-ttu-id="fded6-114">例如，以下示例将触发 **美国银行帐户号** 策略：检查帐户78344011</span><span class="sxs-lookup"><span data-stu-id="fded6-114">For example, the following sample would trigger for the **US Bank Account Number** policy: Checking Account 78344011</span></span>

<span data-ttu-id="fded6-115">若要详细了解为你的内容检测 **美国银行帐号** 所需的内容，请参阅本文中的以下部分： [这些敏感信息类型对美国银行帐号的外观](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span><span class="sxs-lookup"><span data-stu-id="fded6-115">For more information on what is required for a **US Bank Account Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US Bank Account Number](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)</span></span>
  
<span data-ttu-id="fded6-116">使用不同的内置敏感信息类型，请参阅以下文章，了解其他类型所需的信息： [敏感信息类型查找的内容](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="fded6-116">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span></span>
  