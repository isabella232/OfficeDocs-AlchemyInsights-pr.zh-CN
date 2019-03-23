---
title: 还原已删除的网站集
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 5/1/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 1f9a66daf7bee43291b785b6260aec8725ee782f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753776"
---
# <a name="restore-a-deleted-site-collection"></a><span data-ttu-id="74613-102">还原已删除的网站集</span><span class="sxs-lookup"><span data-stu-id="74613-102">Restore a deleted site collection</span></span>

<span data-ttu-id="74613-103">当管理员删除经典网站集时, 它将放在网站集回收站中, 在这种情况下, 它将保留93天, 然后才会被永久删除。</span><span class="sxs-lookup"><span data-stu-id="74613-103">When an admin deletes a classic site collection, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="74613-104">若要还原网站集, 请执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="74613-104">To restore the site collection:</span></span>
  
1. <span data-ttu-id="74613-105">在经典 SharePoint 管理中心中, 单击功能区上的 "**回收站**"。</span><span class="sxs-lookup"><span data-stu-id="74613-105">In the classic SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="74613-106">选中要还原的网站集旁边的复选框。</span><span class="sxs-lookup"><span data-stu-id="74613-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="74613-107">单击 "**还原已删除的项目**"。</span><span class="sxs-lookup"><span data-stu-id="74613-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="74613-108">若要还原已删除的通信网站, 可以使用新的 SharePoint 管理中心预览。</span><span class="sxs-lookup"><span data-stu-id="74613-108">To restore a deleted communication site, you can use the new SharePoint admin center preview.</span></span> <span data-ttu-id="74613-109">否则, 您需要使用 PowerShell。</span><span class="sxs-lookup"><span data-stu-id="74613-109">Otherwise, you need to use PowerShell.</span></span> <span data-ttu-id="74613-110">若要还原属于 Office 365 组的网站, 需要在 Exchange 管理中心内还原该组。</span><span class="sxs-lookup"><span data-stu-id="74613-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="74613-111">组可以在删除后30天内还原。</span><span class="sxs-lookup"><span data-stu-id="74613-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

