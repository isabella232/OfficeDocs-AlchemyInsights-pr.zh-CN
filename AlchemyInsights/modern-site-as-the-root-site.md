---
title: 新式网站作为根网站
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: d5ea73c967013822854dbd408d4628d991c90378
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620749"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="e8ac5-102">新式网站作为根网站</span><span class="sxs-lookup"><span data-stu-id="e8ac5-102">Modern site as root site</span></span>

<span data-ttu-id="e8ac5-103">我们已经开始推出新功能, 使你能够将经典网站根网站替换为新式网站。</span><span class="sxs-lookup"><span data-stu-id="e8ac5-103">We have begun to rollout a new feature that will allow you to swap your classic site root site with a modern site.</span></span> <span data-ttu-id="e8ac5-104">使用[SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)可在存档原始网站的同时, 将网站的位置替换为其他网站。</span><span class="sxs-lookup"><span data-stu-id="e8ac5-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="e8ac5-105">可用于两个工作组网站 (未连接到组) 和通信网站。</span><span class="sxs-lookup"><span data-stu-id="e8ac5-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

>[!Important]
> <span data-ttu-id="e8ac5-106">请勿删除经典根网站来创建新式通信网站。</span><span class="sxs-lookup"><span data-stu-id="e8ac5-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="e8ac5-107">Microsoft 不支持这种情况。</span><span class="sxs-lookup"><span data-stu-id="e8ac5-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="e8ac5-108">删除根网站将使组织中的所有 SharePoint 网站对所有用户不可访问, 直到您还原网站或在相同的 URL 上创建新网站。</span><span class="sxs-lookup"><span data-stu-id="e8ac5-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="e8ac5-109">我们将通过消息中心传达此功能。</span><span class="sxs-lookup"><span data-stu-id="e8ac5-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="e8ac5-110">你应该会在你的租户中很快启用此功能。</span><span class="sxs-lookup"><span data-stu-id="e8ac5-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="e8ac5-111">交换网站的已知问题</span><span class="sxs-lookup"><span data-stu-id="e8ac5-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="e8ac5-112">目标网站可能会在短时间内返回 "未找到" (HTTP 404) 错误。</span><span class="sxs-lookup"><span data-stu-id="e8ac5-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="e8ac5-113">需要重新爬网内容才能更新搜索索引。</span><span class="sxs-lookup"><span data-stu-id="e8ac5-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="e8ac5-114">此处不需要手动步骤, 这将自动完成。</span><span class="sxs-lookup"><span data-stu-id="e8ac5-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="e8ac5-115">依赖于 "静态" 链接的任何内容 (如文件同步和 OneNote 文件) 都需要手动更正。</span><span class="sxs-lookup"><span data-stu-id="e8ac5-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="e8ac5-116">可能需要验证 Project Server 网站, 以确保它们仍正确关联。</span><span class="sxs-lookup"><span data-stu-id="e8ac5-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
