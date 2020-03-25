---
title: 将选项迁移到 SharePoint Online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932720"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="7fec0-102">将选项迁移到 SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="7fec0-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="7fec0-103">**重要说明**：许多 SharePoint Online 和 OneDrive 客户对在后台运行的服务运行关键业务应用程序。</span><span class="sxs-lookup"><span data-stu-id="7fec0-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="7fec0-104">其中包括内容迁移、数据丢失防护（DLP）和备份解决方案。</span><span class="sxs-lookup"><span data-stu-id="7fec0-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="7fec0-105">在这些前所未有的时间内，我们将采取措施，以确保在远程工作方案中，SharePoint Online 和 OneDrive 服务对依赖于该服务的用户保持高可用性和可靠性。</span><span class="sxs-lookup"><span data-stu-id="7fec0-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="7fec0-106">为支持此目标，我们已在工作日白天营业时对后台应用（迁移、DLP 和备份解决方案）实施了更严格的限制限制。</span><span class="sxs-lookup"><span data-stu-id="7fec0-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="7fec0-107">在这些情况中，您应认为这些应用程序的吞吐量非常有限。</span><span class="sxs-lookup"><span data-stu-id="7fec0-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="7fec0-108">但是，在夜间和周末的时间内，服务将准备好处理来自后台应用程序的较大数量的请求。</span><span class="sxs-lookup"><span data-stu-id="7fec0-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="7fec0-109">**迁移选项**</span><span class="sxs-lookup"><span data-stu-id="7fec0-109">**Migration options**</span></span>

<span data-ttu-id="7fec0-110">有不同的选项可用于将内容迁移到 SharePoint Online，具体取决于您需要移动的文件的大小和数量，请参阅[此处](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online)的选项列表。</span><span class="sxs-lookup"><span data-stu-id="7fec0-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="7fec0-111">有关内容迁移的详细信息，请访问下面的链接。</span><span class="sxs-lookup"><span data-stu-id="7fec0-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="7fec0-112">Sharepoint 迁移工具</span><span class="sxs-lookup"><span data-stu-id="7fec0-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="7fec0-113">迁移管理器入门</span><span class="sxs-lookup"><span data-stu-id="7fec0-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="7fec0-114">Sharepoint Online 和 ODB 迁移速度</span><span class="sxs-lookup"><span data-stu-id="7fec0-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="7fec0-115">避免在 SharePoint Online 中受限或遭屏蔽</span><span class="sxs-lookup"><span data-stu-id="7fec0-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="7fec0-116">SharePoint 迁移评估工具（SMAT）</span><span class="sxs-lookup"><span data-stu-id="7fec0-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="7fec0-117">**注意**：当前 sharepoint 迁移工具仅支持从 SharePoint 2010 和2013迁移。</span><span class="sxs-lookup"><span data-stu-id="7fec0-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="7fec0-118">目前不支持版本2016或2019。</span><span class="sxs-lookup"><span data-stu-id="7fec0-118">Version 2016 or 2019 are not supported at this time.</span></span>
