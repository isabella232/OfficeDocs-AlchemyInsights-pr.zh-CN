---
title: DLP 策略提示无法正常工作
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932576"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="b8e25-102">DLP 策略提示问题</span><span class="sxs-lookup"><span data-stu-id="b8e25-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="b8e25-103">**重要说明**：许多 SharePoint Online 和 OneDrive 客户对在后台运行的服务运行关键业务应用程序。</span><span class="sxs-lookup"><span data-stu-id="b8e25-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b8e25-104">其中包括内容迁移、数据丢失防护（DLP）和备份解决方案。</span><span class="sxs-lookup"><span data-stu-id="b8e25-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b8e25-105">在这些前所未有的时间内，我们将采取措施，以确保在远程工作方案中，SharePoint Online 和 OneDrive 服务对依赖于该服务的用户保持高可用性和可靠性。</span><span class="sxs-lookup"><span data-stu-id="b8e25-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b8e25-106">为支持此目标，我们已在工作日白天营业时对后台应用（迁移、DLP 和备份解决方案）实施了更严格的限制限制。</span><span class="sxs-lookup"><span data-stu-id="b8e25-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b8e25-107">在这些情况中，您应认为这些应用程序的吞吐量非常有限。</span><span class="sxs-lookup"><span data-stu-id="b8e25-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b8e25-108">但是，在夜间和周末的时间内，服务将准备好处理来自后台应用程序的较大数量的请求。</span><span class="sxs-lookup"><span data-stu-id="b8e25-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b8e25-109">**DLP 策略提示**</span><span class="sxs-lookup"><span data-stu-id="b8e25-109">**DLP policy tips**</span></span>

<span data-ttu-id="b8e25-110">使用**DLP 策略**时，用户可以收到策略**提示**冲突的通知。</span><span class="sxs-lookup"><span data-stu-id="b8e25-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="b8e25-111">管理员可以配置在测试其 DLP 策略时或策略处于完全强制模式时显示的策略提示。</span><span class="sxs-lookup"><span data-stu-id="b8e25-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="b8e25-112">若要在完全强制模式下的安全与合规中心中的 DLP 策略上配置策略提示，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="b8e25-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="b8e25-113">使用[此处](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)的步骤，确保已在 DLP 规则上**启用**策略提示。</span><span class="sxs-lookup"><span data-stu-id="b8e25-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="b8e25-114">确保您的内容与在[此处](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)触发本文中所述规则**所需**的**内容相匹配**。</span><span class="sxs-lookup"><span data-stu-id="b8e25-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="b8e25-115">在 OWA 和 Outlook 中显示策略提示。</span><span class="sxs-lookup"><span data-stu-id="b8e25-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="b8e25-116">但是，使用**Outlook 2013 或更高版本**时，策略提示仅在特定条件下显示。</span><span class="sxs-lookup"><span data-stu-id="b8e25-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="b8e25-117">下面列出了这些条件：[适用于 Outlook 2013 或更高版本的支持条件，用于显示策略提示](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="b8e25-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="b8e25-118">有关 DLP 策略提示的详细信息，请参阅：[显示策略提示的 dlp](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)策略</span><span class="sxs-lookup"><span data-stu-id="b8e25-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  