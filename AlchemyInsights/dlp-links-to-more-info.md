---
title: 有关 DLP 问题的详细信息
ms.author: pebaum
author: pebaum
manager: laurawi
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2447"
- "3200001"
ms.openlocfilehash: 6525cee0555f1ae67b7d4e32445b9a1537d4a804
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932684"
---
# <a name="information-about-dlp-issues"></a><span data-ttu-id="a36de-102">有关 DLP 问题的信息</span><span class="sxs-lookup"><span data-stu-id="a36de-102">Information about DLP issues</span></span>

<span data-ttu-id="a36de-103">**重要说明**：许多 SharePoint Online 和 OneDrive 客户对在后台运行的服务运行关键业务应用程序。</span><span class="sxs-lookup"><span data-stu-id="a36de-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="a36de-104">其中包括内容迁移、数据丢失防护（DLP）和备份解决方案。</span><span class="sxs-lookup"><span data-stu-id="a36de-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="a36de-105">在这些前所未有的时间内，我们将采取措施，以确保在远程工作方案中，SharePoint Online 和 OneDrive 服务对依赖于该服务的用户保持高可用性和可靠性。</span><span class="sxs-lookup"><span data-stu-id="a36de-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="a36de-106">为支持此目标，我们已在工作日白天营业时对后台应用（迁移、DLP 和备份解决方案）实施了更严格的限制限制。</span><span class="sxs-lookup"><span data-stu-id="a36de-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="a36de-107">在这些情况中，您应认为这些应用程序的吞吐量非常有限。</span><span class="sxs-lookup"><span data-stu-id="a36de-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="a36de-108">但是，在夜间和周末的时间内，服务将准备好处理来自后台应用程序的较大数量的请求。</span><span class="sxs-lookup"><span data-stu-id="a36de-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="a36de-109">**有关 DLP 策略的信息**</span><span class="sxs-lookup"><span data-stu-id="a36de-109">**Information on DLP policy**</span></span>

<span data-ttu-id="a36de-110">使用 DLP 策略，可以识别、监视和自动保护跨 Office 365 的敏感信息。</span><span class="sxs-lookup"><span data-stu-id="a36de-110">With a DLP policy, you can identify, monitor, and automatically protect sensitive information across Office 365.</span></span>

<span data-ttu-id="a36de-111">有关详细信息，请访问以下链接：</span><span class="sxs-lookup"><span data-stu-id="a36de-111">Please visit these links for more information:</span></span>

- [<span data-ttu-id="a36de-112">数据丢失防护概述</span><span class="sxs-lookup"><span data-stu-id="a36de-112">Overview of data loss prevention</span></span>](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies)
- [<span data-ttu-id="a36de-113">敏感信息类型查找什么</span><span class="sxs-lookup"><span data-stu-id="a36de-113">What the sensitive information types look for</span></span>](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
- [<span data-ttu-id="a36de-114">创建自定义敏感信息类型</span><span class="sxs-lookup"><span data-stu-id="a36de-114">Create a custom sensitive information type</span></span>](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)
- [<span data-ttu-id="a36de-115">发送电子邮件通知并显示策略提示</span><span class="sxs-lookup"><span data-stu-id="a36de-115">Send email notifications and show policy tips</span></span>](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
- [<span data-ttu-id="a36de-116">使用保留标签和 DLP 保护 SharePoint Online 文件</span><span class="sxs-lookup"><span data-stu-id="a36de-116">Protect SharePoint Online files with retention labels and DLP</span></span>](https://docs.microsoft.com/office365/securitycompliance/protect-sharepoint-online-files-with-office-365-labels-and-dlp)
- [<span data-ttu-id="a36de-117">DLP 和 Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a36de-117">DLP and Microsoft Teams</span></span>](https://docs.microsoft.com/office365/securitycompliance/dlp-microsoft-teams)

<span data-ttu-id="a36de-118">若要使用内置或自定义的敏感信息类型测试数据，请使用 "**分类** > **敏感信息类型**" 下的 "**测试类型**" 选项。</span><span class="sxs-lookup"><span data-stu-id="a36de-118">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="a36de-119">有关详细信息，请参阅[测试自定义敏感信息类型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)。</span><span class="sxs-lookup"><span data-stu-id="a36de-119">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>