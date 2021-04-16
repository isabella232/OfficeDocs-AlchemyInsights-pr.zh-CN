---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51770981"
---
# <a name="verify-your-domain"></a><span data-ttu-id="fc368-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="fc368-102">Verify your domain</span></span>

 <span data-ttu-id="fc368-103">**记录可能尚未通过 Internet 更新。**</span><span class="sxs-lookup"><span data-stu-id="fc368-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="fc368-104">通常只需几分钟，我们就能看到新记录，但有时可能需要几个小时。</span><span class="sxs-lookup"><span data-stu-id="fc368-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="fc368-105">如果已经等待了那么长时间，请仔细检查是否将准确值复制并粘贴到 DNS 主机的 TXT 验证记录中。</span><span class="sxs-lookup"><span data-stu-id="fc368-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="fc368-106">一个常见的问题是未包含记录的 "MS=" 部分。</span><span class="sxs-lookup"><span data-stu-id="fc368-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="fc368-107">我们也需要的！</span><span class="sxs-lookup"><span data-stu-id="fc368-107">We need that too!</span></span>

- <span data-ttu-id="fc368-108">在一些 DNS 主机上，你需要采取额外步骤来保存区域文件（存储 DNS记录的地方），以便它将通过 Internet 更新。</span><span class="sxs-lookup"><span data-stu-id="fc368-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="fc368-109">确保你已保存更改，以便 Microsoft 可以看到并验证记录。</span><span class="sxs-lookup"><span data-stu-id="fc368-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
