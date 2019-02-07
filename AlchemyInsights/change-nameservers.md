---
title: 更改名称服务器
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d011531a-0951-49c0-af30-40d2e765f381
ms.openlocfilehash: 61c4c5e43a247679bf18fd3861dd98fbe9a7b3eb
ms.sourcegitcommit: 5dee2fcb492bd922092a6de8045a95febe57b97e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2019
ms.locfileid: "29758694"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="20fbd-102">将域名称服务器更新为 Office 365</span><span class="sxs-lookup"><span data-stu-id="20fbd-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="20fbd-103">注意： 名称服务器更改有时需要花 48 小时传播。</span><span class="sxs-lookup"><span data-stu-id="20fbd-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="20fbd-p101">若要在 Office 365 中设置域，需要更新注册机构中的名称服务器。创建或编辑域注册机构中的名称服务器记录。</span><span class="sxs-lookup"><span data-stu-id="20fbd-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="20fbd-106">转到域注册机构的网站，查找可在其中编辑名称服务器的区域。</span><span class="sxs-lookup"><span data-stu-id="20fbd-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
    
2. <span data-ttu-id="20fbd-107">创建或编辑两个名称服务器记录，匹配以下值：</span><span class="sxs-lookup"><span data-stu-id="20fbd-107">Create or edit two nameserver records to match these values:</span></span>
    
  - <span data-ttu-id="20fbd-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="20fbd-108">ns1.bdm.microsoftonline.com</span></span>
    
  - <span data-ttu-id="20fbd-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="20fbd-109">ns2.bdm.microsoftonline.com</span></span>
    
3. <span data-ttu-id="20fbd-110">保存更改。</span><span class="sxs-lookup"><span data-stu-id="20fbd-110">Save changes.</span></span>
    
<span data-ttu-id="20fbd-111">还可在本文中查看详细的说明：[更改名称服务器以使用任意域名注册机构设置 Office 365](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="20fbd-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  

