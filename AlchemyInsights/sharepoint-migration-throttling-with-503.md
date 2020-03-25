---
title: 包含503错误的 SharePoint 迁移限制
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931648"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="8a7c8-102">包含503错误的 SharePoint 迁移限制</span><span class="sxs-lookup"><span data-stu-id="8a7c8-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="8a7c8-103">**重要说明**：许多 SharePoint Online 和 OneDrive 客户对在后台运行的服务运行关键业务应用程序。</span><span class="sxs-lookup"><span data-stu-id="8a7c8-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="8a7c8-104">其中包括内容迁移、数据丢失防护（DLP）和备份解决方案。</span><span class="sxs-lookup"><span data-stu-id="8a7c8-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="8a7c8-105">在这些前所未有的时间内，我们将采取措施，以确保在远程工作方案中，SharePoint Online 和 OneDrive 服务对依赖于该服务的用户保持高可用性和可靠性。</span><span class="sxs-lookup"><span data-stu-id="8a7c8-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="8a7c8-106">为支持此目标，我们已在工作日白天营业时对后台应用（迁移、DLP 和备份解决方案）实施了更严格的限制限制。</span><span class="sxs-lookup"><span data-stu-id="8a7c8-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="8a7c8-107">在这些情况中，您应认为这些应用程序的吞吐量非常有限。</span><span class="sxs-lookup"><span data-stu-id="8a7c8-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="8a7c8-108">但是，在夜间和周末的时间内，服务将准备好处理来自后台应用程序的较大数量的请求。</span><span class="sxs-lookup"><span data-stu-id="8a7c8-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="8a7c8-109">**503迁移到 SharePoint Online 时出现的错误**</span><span class="sxs-lookup"><span data-stu-id="8a7c8-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="8a7c8-110">它似乎正在迁移到 SharePoint Online 并收到503错误。</span><span class="sxs-lookup"><span data-stu-id="8a7c8-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="8a7c8-111">请按照下面的步骤操作，以便我们能够尽快为你提供帮助。</span><span class="sxs-lookup"><span data-stu-id="8a7c8-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="8a7c8-112">单击 "**联系人支持**"，然后单击 "**新建服务请求**"。</span><span class="sxs-lookup"><span data-stu-id="8a7c8-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="8a7c8-113">对于 "标题" 和 "说明"，请**使用503键入 SharePoint 迁移限制**。</span><span class="sxs-lookup"><span data-stu-id="8a7c8-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="8a7c8-114">提交票证后，请使用以下信息对其进行更新：</span><span class="sxs-lookup"><span data-stu-id="8a7c8-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="8a7c8-115">迁移的剩余量（例如，多少 Tb？）。</span><span class="sxs-lookup"><span data-stu-id="8a7c8-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="8a7c8-116">迁移开始和结束日期。</span><span class="sxs-lookup"><span data-stu-id="8a7c8-116">Migration start and end date.</span></span>
    - <span data-ttu-id="8a7c8-117">描述从中迁移内容的位置，如 SharePoint Server、Box、GDrive、文件共享等。</span><span class="sxs-lookup"><span data-stu-id="8a7c8-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="8a7c8-118">估计限制错误的数量（例如，每小时 x 限制值？）和限制发生的时间。</span><span class="sxs-lookup"><span data-stu-id="8a7c8-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="8a7c8-119">您使用的是哪种迁移工具（例如，SPMT 或 ShareGate）。</span><span class="sxs-lookup"><span data-stu-id="8a7c8-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


