---
title: DLP 未如预期工作
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
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707800"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="995b4-102">DLP 未如预期工作</span><span class="sxs-lookup"><span data-stu-id="995b4-102">DLP not working as expected</span></span>

<span data-ttu-id="995b4-103">**重要信息：** 在这段前所未有的时期，我们正在采取措施确保 SharePoint Online 和 OneDrive 服务高度可用，请访问 [SharePoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)，获取详细信息。</span><span class="sxs-lookup"><span data-stu-id="995b4-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="995b4-104">**设置 DLP**</span><span class="sxs-lookup"><span data-stu-id="995b4-104">**Setting up DLP**</span></span>

<span data-ttu-id="995b4-105">Office 365 中的 **数据丢失防护 (DLP)** 是否未如预期工作？</span><span class="sxs-lookup"><span data-stu-id="995b4-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="995b4-106">如果是，请确保 **DLP** 策略设置正确，并且数据包含 **DLP** 策略在评估时正在查找的内容。</span><span class="sxs-lookup"><span data-stu-id="995b4-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="995b4-107">DLP 策略允许您标识和保护您组织的敏感信息。</span><span class="sxs-lookup"><span data-stu-id="995b4-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="995b4-108">若要设置 DLP 策略，请使用此处 [的信息](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)。</span><span class="sxs-lookup"><span data-stu-id="995b4-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="995b4-109">**DLP 策略查找什么**</span><span class="sxs-lookup"><span data-stu-id="995b4-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="995b4-110">在安全与合规中心内使用内置敏感信息类型时，DLP 策略在检测这些敏感信息类型时会查找特定模式和元素。</span><span class="sxs-lookup"><span data-stu-id="995b4-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="995b4-111">**内置敏感信息类型**</span><span class="sxs-lookup"><span data-stu-id="995b4-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="995b4-112">有关内置敏感类型以及 DLP 策略在检测敏感类型时查找的信息，请参阅：敏感信息类型 [查找什么](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)。</span><span class="sxs-lookup"><span data-stu-id="995b4-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="995b4-113">**自定义敏感信息类型**</span><span class="sxs-lookup"><span data-stu-id="995b4-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="995b4-114">如果您尝试创建自定义敏感信息类型，请使用以下文章来了解如何创建自定义敏感信息类型： [创建自定义敏感信息类型](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)。</span><span class="sxs-lookup"><span data-stu-id="995b4-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="995b4-115">**测试 DLP 策略**</span><span class="sxs-lookup"><span data-stu-id="995b4-115">**Test a DLP policy**</span></span>

<span data-ttu-id="995b4-116">若要使用内置或自定义敏感信息类型测试数据，请使用分类敏感信息类型下的"测试  >  **类型"选项**。</span><span class="sxs-lookup"><span data-stu-id="995b4-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="995b4-117">有关详细信息，请参阅["测试自定义敏感信息类型"。](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)</span><span class="sxs-lookup"><span data-stu-id="995b4-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="995b4-118">**报表**</span><span class="sxs-lookup"><span data-stu-id="995b4-118">**Reports**</span></span>
  
- <span data-ttu-id="995b4-119">使用 DLP 报告获取 [敏感数据见解。](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="995b4-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="995b4-120">使用事件报告查看事件 [的特定详细信息](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)。</span><span class="sxs-lookup"><span data-stu-id="995b4-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
