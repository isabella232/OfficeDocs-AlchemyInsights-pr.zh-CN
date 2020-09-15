---
title: 更改名称服务器
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 07a0dd19a768dd2b97923f0ced566b69ca2d6ba7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714678"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="034c2-102">将域名称服务器更新为指向 Microsoft</span><span class="sxs-lookup"><span data-stu-id="034c2-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="034c2-103">注意：名称服务器更改有时候需要长达 48 小时才能进行传播。</span><span class="sxs-lookup"><span data-stu-id="034c2-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="034c2-p101">若要在 Microsoft 365 中设置域，需要更新注册机构处的名称服务器。创建或编辑域注册机构处的名称服务器记录。</span><span class="sxs-lookup"><span data-stu-id="034c2-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="034c2-106">转到域注册机构的网站，查找可在其中编辑名称服务器的区域。</span><span class="sxs-lookup"><span data-stu-id="034c2-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="034c2-107">创建或编辑两个名称服务器记录，匹配以下值：</span><span class="sxs-lookup"><span data-stu-id="034c2-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="034c2-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="034c2-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="034c2-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="034c2-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="034c2-110">保存更改。</span><span class="sxs-lookup"><span data-stu-id="034c2-110">Save changes.</span></span>

<span data-ttu-id="034c2-111">还可以在下面这篇文章中查找详细说明：[通过任意域注册机构更改名称服务器](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="034c2-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  