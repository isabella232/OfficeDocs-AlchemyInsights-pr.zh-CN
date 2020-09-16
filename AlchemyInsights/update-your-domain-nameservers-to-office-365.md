---
title: 将域名称服务器更新为指向 Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734901"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="539fb-102">将域名称服务器更新为指向 Microsoft</span><span class="sxs-lookup"><span data-stu-id="539fb-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="539fb-103">注意：名称服务器更改有时候需要长达 48 小时才能进行传播。</span><span class="sxs-lookup"><span data-stu-id="539fb-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="539fb-104">若要使用 Microsoft 设置你的域，你的注册机构上的名称服务器需要更新。</span><span class="sxs-lookup"><span data-stu-id="539fb-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="539fb-105">创建或编辑域注册机构中的名称服务器记录。</span><span class="sxs-lookup"><span data-stu-id="539fb-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="539fb-106">转到域注册机构的网站，查找可在其中编辑名称服务器的区域。</span><span class="sxs-lookup"><span data-stu-id="539fb-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="539fb-107">创建或编辑两个名称服务器记录，匹配以下值：</span><span class="sxs-lookup"><span data-stu-id="539fb-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="539fb-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="539fb-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="539fb-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="539fb-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="539fb-110">保存更改。</span><span class="sxs-lookup"><span data-stu-id="539fb-110">Save changes.</span></span>

<span data-ttu-id="539fb-111">您还可以在本文中查找详细说明： [更改名称服务器以使用任何域注册机构设置 Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="539fb-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  