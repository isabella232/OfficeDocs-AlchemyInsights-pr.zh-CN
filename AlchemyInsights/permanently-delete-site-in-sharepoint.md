---
title: 永久删除 SharePoint 中的站点
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955108"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="48f89-102">永久删除 SharePoint 中的站点</span><span class="sxs-lookup"><span data-stu-id="48f89-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="48f89-103">如要重新使用已删除站点的 URL（来重新创建站点），或永久删除不再使用的站点，可使用新版 SharePoint 管理中心中的“**永久删除**”。 </span><span class="sxs-lookup"><span data-stu-id="48f89-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="48f89-104">转到[删除新版 SharePoint 管理中心的站点页面](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)，然后使用在组织中具有管理员权限的帐户进行登录。</span><span class="sxs-lookup"><span data-stu-id="48f89-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="48f89-105">在左栏中，选择一个站点。</span><span class="sxs-lookup"><span data-stu-id="48f89-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="48f89-106">单击**永久删除**。</span><span class="sxs-lookup"><span data-stu-id="48f89-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="48f89-107">**注意**：连接到组的站点无法永久从新版 SharePoint 管理中心中删除。</span><span class="sxs-lookup"><span data-stu-id="48f89-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="48f89-108">系统将替代使用 [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite)。</span><span class="sxs-lookup"><span data-stu-id="48f89-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="48f89-109">有关详细信息，请参阅[永久删除站点](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site)。</span><span class="sxs-lookup"><span data-stu-id="48f89-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
