---
title: 在 SharePoint Online 中管理搜索架构
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 9836cf139e97fc556995a8f0ad38c51c5c2392ac
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40042953"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="1171c-102">在 SharePoint Online 中管理搜索架构</span><span class="sxs-lookup"><span data-stu-id="1171c-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="1171c-103">搜索架构可控制用户可以搜索的内容、用户可以搜索的内容以及在搜索网站上显示结果的方式。</span><span class="sxs-lookup"><span data-stu-id="1171c-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="1171c-104">请参阅[在 SharePoint Online 中管理搜索架构](https://docs.microsoft.com/sharepoint/manage-search-schema)，了解如何执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="1171c-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="1171c-105">更改搜索架构。</span><span class="sxs-lookup"><span data-stu-id="1171c-105">Change the search schema.</span></span>
- <span data-ttu-id="1171c-106">创建托管属性。</span><span class="sxs-lookup"><span data-stu-id="1171c-106">Create managed properties.</span></span>
- <span data-ttu-id="1171c-107">将已爬网映射的已爬网属性映射到托管属性。</span><span class="sxs-lookup"><span data-stu-id="1171c-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="1171c-108">请注意以下关于管理搜索架构的内容：</span><span class="sxs-lookup"><span data-stu-id="1171c-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="1171c-109">如果您收到一条警告，指出在进行架构更改时**应用程序已暂停**，这只是临时发生，因为存在服务维护。</span><span class="sxs-lookup"><span data-stu-id="1171c-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="1171c-110">如果超过了24小时，但仍遇到警告，请记录一种支持案例。</span><span class="sxs-lookup"><span data-stu-id="1171c-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="1171c-111">当您更改托管属性或添加新属性时，更改将仅在重新对内容进行爬网后才会生效。</span><span class="sxs-lookup"><span data-stu-id="1171c-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="1171c-112">在 SharePoint Online 中，爬网会根据定义的爬网计划自动进行。</span><span class="sxs-lookup"><span data-stu-id="1171c-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="1171c-113">若要确保对所做的更改进行爬网，您可以专门[请求对列表或库重新编制索引](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="1171c-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="1171c-114">有关搜索架构的完整概述，请参阅[简介搜索架构](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="1171c-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


