---
title: SharePoint Online 中的搜索
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f790efbe6ed445786933efa3fc980f974693d1d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770757"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="ac9b1-102">SharePoint Online 中的内容爬网和索引</span><span class="sxs-lookup"><span data-stu-id="ac9b1-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="ac9b1-103">必须对内容进行爬网并将其添加到搜索索引中，以便用户能够在 SharePoint Online 中查找他们搜索的内容。</span><span class="sxs-lookup"><span data-stu-id="ac9b1-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span>

- <span data-ttu-id="ac9b1-104">确保可 [搜索网站内容](https://docs.microsoft.com/sharepoint/make-site-content-searchable)，从而找到内容。</span><span class="sxs-lookup"><span data-stu-id="ac9b1-104">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="ac9b1-105">更改托管属性或更改已爬网和托管属性的映射后，必须重新对网站进行爬网，然后才能在搜索索引中反映您所做的更改。</span><span class="sxs-lookup"><span data-stu-id="ac9b1-105">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span>

- <span data-ttu-id="ac9b1-106">有关详细信息，请参阅 [手动对网站、库或列表的请求爬网和重新编制索引](https://docs.microsoft.com/sharepoint/crawl-site-content)。</span><span class="sxs-lookup"><span data-stu-id="ac9b1-106">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span>

- <span data-ttu-id="ac9b1-107">在手动请求爬网和完全重新索引以查看是否仍遇到问题后，请至少等待24小时。</span><span class="sxs-lookup"><span data-stu-id="ac9b1-107">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span>

- <span data-ttu-id="ac9b1-108">如果在你启动爬网和完全重新索引后超过了24小时，请记录一个支持案例。</span><span class="sxs-lookup"><span data-stu-id="ac9b1-108">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="ac9b1-109">在许多情况下，我们已经在研究解决方案。</span><span class="sxs-lookup"><span data-stu-id="ac9b1-109">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="ac9b1-110">请至少为我们提供24小时的时间来完成解决方案。</span><span class="sxs-lookup"><span data-stu-id="ac9b1-110">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="ac9b1-111">**重要说明**：如果网站、文档 (库) 或列表已删除且仍显示在搜索结果中，则用户在尝试访问它时，将收到 **错误404文件 "未找到** "。</span><span class="sxs-lookup"><span data-stu-id="ac9b1-111">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="ac9b1-112">应将此问题作为进一步调查的支持案例进行记录。</span><span class="sxs-lookup"><span data-stu-id="ac9b1-112">This issue should be logged as a support case for further investigation.</span></span>



