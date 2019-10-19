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
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36742157"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="d22e8-102">将域名称服务器更新为 Office 365</span><span class="sxs-lookup"><span data-stu-id="d22e8-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="d22e8-103">注意：名称服务器更改有时候需要长达 48 小时才能进行传播。</span><span class="sxs-lookup"><span data-stu-id="d22e8-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="d22e8-p101">若要在 Office 365 中设置域，需要更新注册机构中的名称服务器。创建或编辑域注册机构中的名称服务器记录。</span><span class="sxs-lookup"><span data-stu-id="d22e8-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="d22e8-106">转到域注册机构的网站，查找可在其中编辑名称服务器的区域。</span><span class="sxs-lookup"><span data-stu-id="d22e8-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="d22e8-107">创建或编辑两个名称服务器记录，匹配以下值：</span><span class="sxs-lookup"><span data-stu-id="d22e8-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="d22e8-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="d22e8-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="d22e8-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="d22e8-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="d22e8-110">保存更改。</span><span class="sxs-lookup"><span data-stu-id="d22e8-110">Save changes.</span></span>

<span data-ttu-id="d22e8-111">还可在本文中查看详细的说明：[更改名称服务器以使用任意域名注册机构设置 Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="d22e8-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  