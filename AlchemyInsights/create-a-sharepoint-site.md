---
title: 创建 SharePoint 网站
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806929"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="aa651-102">创建 SharePoint 网站</span><span class="sxs-lookup"><span data-stu-id="aa651-102">Create a SharePoint site</span></span>

<span data-ttu-id="aa651-103">在 SharePoint 管理中心中创建或管理 [活动网站](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) 中的网站。</span><span class="sxs-lookup"><span data-stu-id="aa651-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="aa651-104">有关详细信息，请参阅在 [新 SharePoint 管理中心中管理网站](https://docs.microsoft.com/sharepoint/manage-site-creation)。</span><span class="sxs-lookup"><span data-stu-id="aa651-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="aa651-105">几点</span><span class="sxs-lookup"><span data-stu-id="aa651-105">Tips:</span></span>

- <span data-ttu-id="aa651-106">您 **无法** 使用与现有网站相同的 URL 创建网站。</span><span class="sxs-lookup"><span data-stu-id="aa651-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="aa651-107">如果您删除了某个网站，并且希望重新使用该 URL，则可能是已删除的网站仍存在于 " [已删除的网站](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)" 下。</span><span class="sxs-lookup"><span data-stu-id="aa651-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="aa651-108">需要永久删除网站以重新使用 URL。</span><span class="sxs-lookup"><span data-stu-id="aa651-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="aa651-109">若要使用 Powershell 完全删除站点，请参阅 [remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet 示例。</span><span class="sxs-lookup"><span data-stu-id="aa651-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="aa651-110">某些用户可能不能创建网站。</span><span class="sxs-lookup"><span data-stu-id="aa651-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="aa651-111">[请参阅在 SharePoint Online 中管理网站创建](https://docs.microsoft.com/sharepoint/manage-site-creation)。</span><span class="sxs-lookup"><span data-stu-id="aa651-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="aa651-112">在 **创建** 比预期更长的时间，网站可能会变得被卡住。</span><span class="sxs-lookup"><span data-stu-id="aa651-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="aa651-113">如果在你首次看到此问题后过去已经超过24小时，请记录一个支持票证。</span><span class="sxs-lookup"><span data-stu-id="aa651-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="aa651-114">在许多情况下，我们已经在研究解决方案。</span><span class="sxs-lookup"><span data-stu-id="aa651-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="aa651-115">请至少为我们提供24小时的时间来完成解决方案。</span><span class="sxs-lookup"><span data-stu-id="aa651-115">Please give us at least 24 hours to complete a solution.</span></span>
