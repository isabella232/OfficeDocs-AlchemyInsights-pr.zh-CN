---
title: 还原已删除的网站
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
ms.openlocfilehash: 0cf10a3a0effc1774d8a07c5d0be96384362c175
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32369812"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="6bc62-102">还原已删除的网站</span><span class="sxs-lookup"><span data-stu-id="6bc62-102">Restore a deleted site</span></span>

<span data-ttu-id="6bc62-103">当管理员删除网站时, 该网站将放置在网站集回收站中, 在这种情况下, 它将在永久删除前的93天内保留。</span><span class="sxs-lookup"><span data-stu-id="6bc62-103">When an admin deletes a site , it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="6bc62-104">若要还原网站, 请执行以下操作:</span><span class="sxs-lookup"><span data-stu-id="6bc62-104">To restore the site:</span></span>
  
1. <span data-ttu-id="6bc62-105">在新的 SharePoint 管理中心中, 单击功能区上的 "**回收站**"。</span><span class="sxs-lookup"><span data-stu-id="6bc62-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="6bc62-106">选中要还原的网站集旁边的复选框。</span><span class="sxs-lookup"><span data-stu-id="6bc62-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="6bc62-107">单击 "**还原已删除的项目**"。</span><span class="sxs-lookup"><span data-stu-id="6bc62-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="6bc62-108">若要还原已删除的通信网站, 可以使用新的 SharePoint 管理中心。</span><span class="sxs-lookup"><span data-stu-id="6bc62-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="6bc62-109">否则, 您需要使用 Microsoft PowerShell。</span><span class="sxs-lookup"><span data-stu-id="6bc62-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="6bc62-110">若要还原属于 Office 365 组的网站, 需要在 Exchange 管理中心内还原该组。</span><span class="sxs-lookup"><span data-stu-id="6bc62-110">To restore a site that belongs to an Office 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="6bc62-111">组可以在删除后30天内还原。</span><span class="sxs-lookup"><span data-stu-id="6bc62-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

