---
title: 在传输规则中使用 DLP
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: 124b031e2e029b745c66a71f681f57134739eafe
ms.sourcegitcommit: 07725fcaf073f0ac145f98653b989afdb34c5ad0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43915046"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="1ccc7-102">在传输规则中使用 DLP</span><span class="sxs-lookup"><span data-stu-id="1ccc7-102">Using DLP in transport rules</span></span>

<span data-ttu-id="1ccc7-103">若要将数据丢失防护 (DLP) 集成到现有传输中，请在传输规则设置中使用条件“**如果邮件包含...敏感信息**”。</span><span class="sxs-lookup"><span data-stu-id="1ccc7-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="1ccc7-104">**有关详细信息，请参阅：**</span><span class="sxs-lookup"><span data-stu-id="1ccc7-104">**For more details, see:**</span></span>

- <span data-ttu-id="1ccc7-105">在传输规则中集成 DLP 敏感信息类型：[集成敏感信息规则](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules)。</span><span class="sxs-lookup"><span data-stu-id="1ccc7-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="1ccc7-106">你也可以使用规则上的“测试模式”来测试规则（使用或不使用策略测试）。</span><span class="sxs-lookup"><span data-stu-id="1ccc7-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="1ccc7-107">创建规则后，应等待 30 分钟，然后再进行测试。</span><span class="sxs-lookup"><span data-stu-id="1ccc7-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="1ccc7-108">请参阅[测试邮件流/传输规则](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="1ccc7-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="1ccc7-109">**注意**：如果你尝试使用 EAC 中的传输规则实施新的 DLP 策略，请改为使用[安全与合规中心内的 DLP 策略](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="1ccc7-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
