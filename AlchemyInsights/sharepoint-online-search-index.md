---
title: 在 SharePoint Online 中管理搜索词典
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c2960093bb1cfb649c26528c9f671e6d720ff237
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736043"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="8ecbd-102">SharePoint Online 中的搜索</span><span class="sxs-lookup"><span data-stu-id="8ecbd-102">Search in SharePoint Online</span></span>

<span data-ttu-id="8ecbd-103">必须对内容进行爬网并将其添加到搜索索引中, 以便用户能够在 SharePoint Online 中查找他们搜索的内容。</span><span class="sxs-lookup"><span data-stu-id="8ecbd-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="8ecbd-104">根据预定义的爬网计划自动对内容进行爬网 (无法更改爬网计划)。</span><span class="sxs-lookup"><span data-stu-id="8ecbd-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="8ecbd-105">爬网程序选取自上次爬网以来已更改的内容，并更新索引。</span><span class="sxs-lookup"><span data-stu-id="8ecbd-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="8ecbd-106">若要确保对内容进行爬网并更新索引, 请执行以下步骤。</span><span class="sxs-lookup"><span data-stu-id="8ecbd-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="8ecbd-107">确保可搜索网站内容, 从而找到内容。</span><span class="sxs-lookup"><span data-stu-id="8ecbd-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="8ecbd-108">有关详细信息, 请参阅[使网站上的内容](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable)可供搜索。</span><span class="sxs-lookup"><span data-stu-id="8ecbd-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="8ecbd-109">更改托管属性或更改已爬网和托管属性的映射后, 必须重新对网站进行爬网, 然后才能在搜索索引中反映您所做的更改。</span><span class="sxs-lookup"><span data-stu-id="8ecbd-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="8ecbd-110">由于您所做的更改是在搜索架构中进行的, 而不是实际网站, 因此爬网程序将不会自动对网站重新编制索引。</span><span class="sxs-lookup"><span data-stu-id="8ecbd-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="8ecbd-111">有关详细信息, 请参阅[手动对网站、库或列表的请求爬网和重新编制索引](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten)。</span><span class="sxs-lookup"><span data-stu-id="8ecbd-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="8ecbd-112">在手动请求爬网和完全重新索引以查看是否仍遇到问题后, 请至少等待24小时。</span><span class="sxs-lookup"><span data-stu-id="8ecbd-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="8ecbd-113">如果在你启动爬网和完全重新索引后超过了24小时, 请记录一个支持案例。</span><span class="sxs-lookup"><span data-stu-id="8ecbd-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="8ecbd-114">在许多情况下, 我们已经在努力解决了解决方案。</span><span class="sxs-lookup"><span data-stu-id="8ecbd-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="8ecbd-115">请至少为我们提供24小时的时间来完成解决方案。</span><span class="sxs-lookup"><span data-stu-id="8ecbd-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="8ecbd-116">**重要说明**: 如果网站、文档 (库) 或列表已删除且仍显示在搜索结果中, 则在尝试访问时, 用户应会收到错误404文件 "未找到"。</span><span class="sxs-lookup"><span data-stu-id="8ecbd-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="8ecbd-117">应将此问题作为进一步调查的支持案例进行记录。</span><span class="sxs-lookup"><span data-stu-id="8ecbd-117">This issue should be logged as a support case for further investigation.</span></span> 



