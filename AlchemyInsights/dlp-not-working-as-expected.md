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
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932612"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="5d5ec-102">DLP 未按预期正常工作</span><span class="sxs-lookup"><span data-stu-id="5d5ec-102">DLP not working as expected</span></span>

<span data-ttu-id="5d5ec-103">**重要说明**：许多 SharePoint Online 和 OneDrive 客户对在后台运行的服务运行关键业务应用程序。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="5d5ec-104">其中包括内容迁移、数据丢失防护（DLP）和备份解决方案。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="5d5ec-105">在这些前所未有的时间内，我们将采取措施，以确保在远程工作方案中，SharePoint Online 和 OneDrive 服务对依赖于该服务的用户保持高可用性和可靠性。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="5d5ec-106">为支持此目标，我们已在工作日白天营业时对后台应用（迁移、DLP 和备份解决方案）实施了更严格的限制限制。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="5d5ec-107">在这些情况中，您应认为这些应用程序的吞吐量非常有限。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="5d5ec-108">但是，在夜间和周末的时间内，服务将准备好处理来自后台应用程序的较大数量的请求。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="5d5ec-109">**设置 DLP**</span><span class="sxs-lookup"><span data-stu-id="5d5ec-109">**Setting up DLP**</span></span>

<span data-ttu-id="5d5ec-110">Office 365 中的**数据丢失防护（DLP）** 是否有问题无法按预期工作？</span><span class="sxs-lookup"><span data-stu-id="5d5ec-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="5d5ec-111">如果是这样，请确保您的**dlp 策略**设置正确，并且您的数据中包含**DLP 策略**在评估时要查找的内容。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="5d5ec-112">DLP 策略允许你标识和保护组织中的敏感信息。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="5d5ec-113">若要设置 DLP 策略，请使用[此处](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)的信息。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="5d5ec-114">**DLP 策略查找的内容**</span><span class="sxs-lookup"><span data-stu-id="5d5ec-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="5d5ec-115">在 Office 365 安全与合规中心中使用**内置的敏感信息类型**时，DLP 策略会在检测这些敏感类型时查找特定模式和元素。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="5d5ec-116">**内置的敏感信息类型**</span><span class="sxs-lookup"><span data-stu-id="5d5ec-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="5d5ec-117">有关内置敏感类型以及在检测敏感类型时 DLP 策略查找的内容的信息，请参阅：[敏感信息类型查找的内容](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="5d5ec-118">**自定义敏感信息类型**</span><span class="sxs-lookup"><span data-stu-id="5d5ec-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="5d5ec-119">如果您尝试创建自定义敏感信息类型，请使用以下文章，了解有关如何创建自定义敏感信息类型的信息：[创建自定义敏感信息类型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="5d5ec-120">**测试 DLP 策略**</span><span class="sxs-lookup"><span data-stu-id="5d5ec-120">**Test a DLP policy**</span></span>

<span data-ttu-id="5d5ec-121">若要使用内置或自定义的敏感信息类型测试数据，请使用 "**分类** > **敏感信息类型**" 下的 "**测试类型**" 选项。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="5d5ec-122">有关详细信息，请参阅[测试自定义敏感信息类型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="5d5ec-123">**报表**</span><span class="sxs-lookup"><span data-stu-id="5d5ec-123">**Reports**</span></span>
  
- <span data-ttu-id="5d5ec-124">使用[DLP 报告](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)获取敏感数据见解。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="5d5ec-125">有关事件[报告](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)的详细信息，请参阅事件的具体详细信息。</span><span class="sxs-lookup"><span data-stu-id="5d5ec-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
