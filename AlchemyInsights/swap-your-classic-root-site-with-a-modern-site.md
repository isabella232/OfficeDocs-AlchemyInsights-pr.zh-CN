---
title: 将经典根网站替换为新式网站
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741534"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="afedd-102">将经典根网站替换为新式网站</span><span class="sxs-lookup"><span data-stu-id="afedd-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="afedd-103">如果您的环境是在2019年4月之前设置的，则可以使用 Microsoft PowerShell 将您的根网站更改为新式网站：</span><span class="sxs-lookup"><span data-stu-id="afedd-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="afedd-104">如果您有一个要用作根网站的不同网站，则可以将[根网站替换（交换）](https://docs.microsoft.com/sharepoint/modern-root-site)到根网站。</span><span class="sxs-lookup"><span data-stu-id="afedd-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="afedd-105">使用[SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)可在存档原始网站的同时，将网站的位置替换为其他网站。</span><span class="sxs-lookup"><span data-stu-id="afedd-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="afedd-106">可用于两个工作组网站（未连接到组）和通信网站。</span><span class="sxs-lookup"><span data-stu-id="afedd-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="afedd-107">将很快引入其他功能，从而使您能够继续使用网站上的内容，但将现有网站转换为通信网站。</span><span class="sxs-lookup"><span data-stu-id="afedd-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="afedd-108">这些功能将逐步推出。</span><span class="sxs-lookup"><span data-stu-id="afedd-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="afedd-109">继续检查消息中心是否有更新。</span><span class="sxs-lookup"><span data-stu-id="afedd-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="afedd-110">交换网站的已知问题</span><span class="sxs-lookup"><span data-stu-id="afedd-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="afedd-111">目标网站可能会在短时间内返回 "未找到" （HTTP 404）错误。</span><span class="sxs-lookup"><span data-stu-id="afedd-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="afedd-112">需要重新爬网内容才能更新搜索索引。</span><span class="sxs-lookup"><span data-stu-id="afedd-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="afedd-113">无需手动执行步骤-这将自动完成。</span><span class="sxs-lookup"><span data-stu-id="afedd-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="afedd-114">依赖于 "静态" 链接的任何内容（如文件同步和 OneNote 文件）都需要手动更正。</span><span class="sxs-lookup"><span data-stu-id="afedd-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="afedd-115">如果源网站是组织的新闻网站，请更新该 URL。</span><span class="sxs-lookup"><span data-stu-id="afedd-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="afedd-116">获取所有组织新闻网站的列表。</span><span class="sxs-lookup"><span data-stu-id="afedd-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="afedd-117">可能需要验证 Project Server 网站，以确保它们仍正确关联。</span><span class="sxs-lookup"><span data-stu-id="afedd-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
