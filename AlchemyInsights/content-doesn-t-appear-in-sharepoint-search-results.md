---
title: 内容未显示在 SharePoint 搜索结果中
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: a57711434d653f5d5667776916c9251bba2370e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713120"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="e2650-102">内容未显示在 SharePoint 搜索结果中</span><span class="sxs-lookup"><span data-stu-id="e2650-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="e2650-103">在搜索结果中不显示预期内容时，请按照以下疑难解答步骤进行操作：</span><span class="sxs-lookup"><span data-stu-id="e2650-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="e2650-104">检查包含预期内容的 **网站** 是否设置为允许内容显示在搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="e2650-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="e2650-105">按照在 [搜索结果中显示网站上的内容](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)中的步骤操作。</span><span class="sxs-lookup"><span data-stu-id="e2650-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="e2650-106">检查包含预期内容的 **列表** 或 **库** 是否设置为允许内容显示在搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="e2650-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="e2650-107">按照 "在 [搜索结果中显示列表或库](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)中的内容" 中的步骤操作。</span><span class="sxs-lookup"><span data-stu-id="e2650-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="e2650-108">验证页面、文档或自定义页面布局是否已发布为 **主要版本。**</span><span class="sxs-lookup"><span data-stu-id="e2650-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="e2650-109">执行搜索中的步骤 3 [不会在 SharePoint Online 中返回所有结果](https://go.microsoft.com/fwlink/?linkid=874525)。</span><span class="sxs-lookup"><span data-stu-id="e2650-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="e2650-110">验证用户是否具有查看内容的 **权限** 。</span><span class="sxs-lookup"><span data-stu-id="e2650-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="e2650-111">按照 [了解 SharePoint 中的权限级别](https://docs.microsoft.com/sharepoint/understanding-permission-levels)中的步骤操作。</span><span class="sxs-lookup"><span data-stu-id="e2650-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="e2650-112">如果已通过添加新的托管属性、编辑托管属性或删除托管属性来更改搜索架构，则将需要请求爬网和重新建立索引。</span><span class="sxs-lookup"><span data-stu-id="e2650-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="e2650-113">按照对[网站、库或列表的手动请求爬网和重新编制索引](https://docs.microsoft.com/sharepoint/crawl-site-content)中的步骤，对内容进行**重新编制索引**。</span><span class="sxs-lookup"><span data-stu-id="e2650-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="e2650-114">这可能需要一段时间，等待24小时后再次检查结果。</span><span class="sxs-lookup"><span data-stu-id="e2650-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="e2650-115">有关详细信息，请参阅 [使网站上的内容](https://docs.microsoft.com/sharepoint/make-site-content-searchable)可供搜索。</span><span class="sxs-lookup"><span data-stu-id="e2650-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
