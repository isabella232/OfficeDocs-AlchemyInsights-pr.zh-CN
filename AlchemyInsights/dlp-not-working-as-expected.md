---
title: DLP 未按预期正常工作
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 574a8a43d8264e98c6af2bfeb1bb472475e6e334
ms.sourcegitcommit: 940169c0edf638b5086d70cc275049f01dcff3cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "42977428"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="2c740-102">DLP 未按预期正常工作</span><span class="sxs-lookup"><span data-stu-id="2c740-102">DLP not working as expected</span></span>

<span data-ttu-id="2c740-103">**重要信息：** 在这段前所未有的时期，我们正在采取措施确保 SharePoint Online 和 OneDrive 服务高度可用，请访问 [SharePoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)，获取详细信息。</span><span class="sxs-lookup"><span data-stu-id="2c740-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="2c740-104">**设置 DLP**</span><span class="sxs-lookup"><span data-stu-id="2c740-104">**Setting up DLP**</span></span>

<span data-ttu-id="2c740-105">Office 365 中的**数据丢失防护（DLP）** 是否有问题无法按预期工作？</span><span class="sxs-lookup"><span data-stu-id="2c740-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="2c740-106">如果是这样，请确保您的**dlp 策略**设置正确，并且您的数据中包含**DLP 策略**在评估时要查找的内容。</span><span class="sxs-lookup"><span data-stu-id="2c740-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="2c740-107">DLP 策略允许你标识和保护组织中的敏感信息。</span><span class="sxs-lookup"><span data-stu-id="2c740-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="2c740-108">若要设置 DLP 策略，请使用[此处](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)的信息。</span><span class="sxs-lookup"><span data-stu-id="2c740-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="2c740-109">**DLP 策略查找的内容**</span><span class="sxs-lookup"><span data-stu-id="2c740-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="2c740-110">在 Office 365 安全与合规中心中使用**内置的敏感信息类型**时，DLP 策略会在检测这些敏感类型时查找特定模式和元素。</span><span class="sxs-lookup"><span data-stu-id="2c740-110">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="2c740-111">**内置的敏感信息类型**</span><span class="sxs-lookup"><span data-stu-id="2c740-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="2c740-112">有关内置敏感类型以及在检测敏感类型时 DLP 策略查找的内容的信息，请参阅：[敏感信息类型查找的内容](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)。</span><span class="sxs-lookup"><span data-stu-id="2c740-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="2c740-113">**自定义敏感信息类型**</span><span class="sxs-lookup"><span data-stu-id="2c740-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="2c740-114">如果您尝试创建自定义敏感信息类型，请使用以下文章，了解有关如何创建自定义敏感信息类型的信息：[创建自定义敏感信息类型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)。</span><span class="sxs-lookup"><span data-stu-id="2c740-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="2c740-115">**测试 DLP 策略**</span><span class="sxs-lookup"><span data-stu-id="2c740-115">**Test a DLP policy**</span></span>

<span data-ttu-id="2c740-116">若要使用内置或自定义的敏感信息类型测试数据，请使用 "**分类** > **敏感信息类型**" 下的 "**测试类型**" 选项。</span><span class="sxs-lookup"><span data-stu-id="2c740-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="2c740-117">有关详细信息，请参阅[测试自定义敏感信息类型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)。</span><span class="sxs-lookup"><span data-stu-id="2c740-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="2c740-118">**报表**</span><span class="sxs-lookup"><span data-stu-id="2c740-118">**Reports**</span></span>
  
- <span data-ttu-id="2c740-119">使用[DLP 报告](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)获取敏感数据见解。</span><span class="sxs-lookup"><span data-stu-id="2c740-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="2c740-120">有关事件[报告](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)的详细信息，请参阅事件的具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="2c740-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
