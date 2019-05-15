---
title: 新式网站作为根网站
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057675"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="28b0a-102">新式网站作为根网站</span><span class="sxs-lookup"><span data-stu-id="28b0a-102">Modern site as root site</span></span>

<span data-ttu-id="28b0a-103">[目标版本](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide)客户现在可以在其 SharePoint 租户的经典根网站上启用新式通信网站体验。</span><span class="sxs-lookup"><span data-stu-id="28b0a-103">[Target Release](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide) customers can now enable the modern communication site experience at the classic root site of their SharePoint tenant.</span></span>

<span data-ttu-id="28b0a-104">可以通过运行一个简单的 PowerShell cmdlet 来激活此功能。</span><span class="sxs-lookup"><span data-stu-id="28b0a-104">This feature can be activated by running a simple PowerShell cmdlet.</span></span> <span data-ttu-id="28b0a-105">在成功执行 PowerShell 命令之后, 根网站将具有新的通信网站主页。</span><span class="sxs-lookup"><span data-stu-id="28b0a-105">On the successful execution of the PowerShell command(s), the root site will have a new communication site home page.</span></span> <span data-ttu-id="28b0a-106">有关 PowerShell cmdlet 和功能要求的详细信息, 请参阅文章[SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps)中提供的。</span><span class="sxs-lookup"><span data-stu-id="28b0a-106">Details about the PowerShell cmdlet and feature requirements are available in the article [Enable-SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps).</span></span> 

<span data-ttu-id="28b0a-107">默认情况下, 我们会逐步将其关闭, 并在 2019 6 月6日结束时2019在全球范围内提供目标版本的客户, 并在全球范围内推出。</span><span class="sxs-lookup"><span data-stu-id="28b0a-107">We'll be gradually rolling this out, off by default, to Targeted Release customers in early May 2019, and the roll out will be available worldwide by the end of June 2019.</span></span> <span data-ttu-id="28b0a-108">继续使用新式的其他新功能引用[消息中心](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)。</span><span class="sxs-lookup"><span data-stu-id="28b0a-108">Continue to refer to the [Message Center](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter) for other new features with Modern.</span></span> 

<span data-ttu-id="28b0a-109">**重要说明**: 请勿删除经典根网站来创建新式通信网站。</span><span class="sxs-lookup"><span data-stu-id="28b0a-109">**Important**: Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="28b0a-110">Microsoft 不支持这种情况。</span><span class="sxs-lookup"><span data-stu-id="28b0a-110">This is not supported by Microsoft.</span></span> <span data-ttu-id="28b0a-111">删除根网站将使组织中的所有 SharePoint 网站对所有用户不可访问, 直到您还原网站或在相同的 URL 上创建新网站。</span><span class="sxs-lookup"><span data-stu-id="28b0a-111">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> 
 
 