---
title: 将域名称服务器更新为 Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.openlocfilehash: 724e9f7501826dc238932ec08e8628d077e20e2c
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918427"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="6efd1-102">将域名称服务器更新为 Office 365</span><span class="sxs-lookup"><span data-stu-id="6efd1-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="6efd1-103">注意： 名称服务器更改有时需要花 48 小时传播。</span><span class="sxs-lookup"><span data-stu-id="6efd1-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="6efd1-p101">若要在 Office 365 中设置域，需要更新注册机构中的名称服务器。创建或编辑域注册机构中的名称服务器记录。</span><span class="sxs-lookup"><span data-stu-id="6efd1-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="6efd1-106">转到域注册机构的网站，查找可在其中编辑名称服务器的区域。</span><span class="sxs-lookup"><span data-stu-id="6efd1-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="6efd1-107">创建或编辑两个名称服务器记录，匹配以下值：</span><span class="sxs-lookup"><span data-stu-id="6efd1-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="6efd1-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="6efd1-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="6efd1-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="6efd1-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="6efd1-110">保存更改。</span><span class="sxs-lookup"><span data-stu-id="6efd1-110">Save changes.</span></span>
    
<span data-ttu-id="6efd1-111">还可在本文中查看详细的说明：[更改名称服务器以使用任意域名注册机构设置 Office 365](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="6efd1-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

