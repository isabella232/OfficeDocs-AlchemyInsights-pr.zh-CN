---
title: 还原已删除的网站
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692033"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="02954-102">还原已删除的网站</span><span class="sxs-lookup"><span data-stu-id="02954-102">Restore a deleted site</span></span>

<span data-ttu-id="02954-103">当管理员删除 SharePoint 网站时，它将放在网站集回收站中，在这种情况下，将在永久删除之前的93天内保留。</span><span class="sxs-lookup"><span data-stu-id="02954-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="02954-104">若要还原网站，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="02954-104">To restore the site:</span></span>
  
1. <span data-ttu-id="02954-105">在新的 SharePoint 管理中心中，单击功能区上的 " **回收站** "。</span><span class="sxs-lookup"><span data-stu-id="02954-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="02954-106">选中要还原的网站集旁边的复选框。</span><span class="sxs-lookup"><span data-stu-id="02954-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="02954-107">单击 " **还原已删除的项目**"。</span><span class="sxs-lookup"><span data-stu-id="02954-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="02954-108">若要还原已删除的通信网站，可以使用新的 SharePoint 管理中心。</span><span class="sxs-lookup"><span data-stu-id="02954-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="02954-109">否则，您需要使用 Microsoft PowerShell。</span><span class="sxs-lookup"><span data-stu-id="02954-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="02954-110">若要还原属于 Microsoft 365 组的网站，需要在 Exchange 管理中心内还原该组。</span><span class="sxs-lookup"><span data-stu-id="02954-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="02954-111">组可以在删除后30天内还原。</span><span class="sxs-lookup"><span data-stu-id="02954-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

