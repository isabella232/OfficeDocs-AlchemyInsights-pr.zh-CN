---
title: SharePoint Online 中的搜索
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: fc49978fbd2c07381dae83061b1a1868cd1df0d0
ms.sourcegitcommit: 327a2c77afc2ff3d67d3aaaea1a92068a3c4bb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/06/2019
ms.locfileid: "36059242"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="96360-102">SharePoint Online 中的搜索</span><span class="sxs-lookup"><span data-stu-id="96360-102">Search in SharePoint Online</span></span>

<span data-ttu-id="96360-103">必须对内容进行爬网并将其添加到搜索索引中, 以便用户能够在 SharePoint Online 中查找他们搜索的内容。</span><span class="sxs-lookup"><span data-stu-id="96360-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="96360-104">根据预定义的爬网计划自动对内容进行爬网 (无法更改爬网计划)。</span><span class="sxs-lookup"><span data-stu-id="96360-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="96360-105">爬网程序选取自上次爬网以来已更改的内容，并更新索引。</span><span class="sxs-lookup"><span data-stu-id="96360-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="96360-106">若要确保对内容进行爬网并更新索引, 请注意以下事项:</span><span class="sxs-lookup"><span data-stu-id="96360-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="96360-107">确保可[搜索网站内容](https://docs.microsoft.com/sharepoint/make-site-content-searchable), 从而找到内容。</span><span class="sxs-lookup"><span data-stu-id="96360-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="96360-108">更改托管属性或更改已爬网和托管属性的映射后, 必须重新对网站进行爬网, 然后才能在搜索索引中反映您所做的更改。</span><span class="sxs-lookup"><span data-stu-id="96360-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="96360-109">由于您所做的更改是在搜索架构中进行的, 而不是实际网站, 因此爬网程序将不会自动对网站重新编制索引。</span><span class="sxs-lookup"><span data-stu-id="96360-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="96360-110">有关详细信息, 请参阅[手动对网站、库或列表的请求爬网和重新编制索引](https://docs.microsoft.com/sharepoint/crawl-site-conten)。</span><span class="sxs-lookup"><span data-stu-id="96360-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="96360-111">在手动请求爬网和完全重新索引以查看是否仍遇到问题后, 请至少等待24小时。</span><span class="sxs-lookup"><span data-stu-id="96360-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="96360-112">如果在你启动爬网和完全重新索引后超过了24小时, 请记录一个支持案例。</span><span class="sxs-lookup"><span data-stu-id="96360-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="96360-113">在许多情况下, 我们已经在努力解决了解决方案。</span><span class="sxs-lookup"><span data-stu-id="96360-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="96360-114">请至少为我们提供24小时的时间来完成解决方案。</span><span class="sxs-lookup"><span data-stu-id="96360-114">Please give us at least 24 hours to complete a solution.</span></span>

>[!重要说明!]<span data-ttu-id="96360-115">: 如果某个网站、文档 (库) 或列表已删除且仍显示在搜索结果中, 则用户在尝试访问它时, 将收到**错误404文件 "找不**到"。</span><span class="sxs-lookup"><span data-stu-id="96360-115">: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="96360-116">应将此问题作为进一步调查的支持案例进行记录。</span><span class="sxs-lookup"><span data-stu-id="96360-116">This issue should be logged as a support case for further investigation.</span></span> 



