---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734296"
---
# <a name="verify-your-domain"></a><span data-ttu-id="9b79b-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="9b79b-102">Verify your domain</span></span>

 <span data-ttu-id="9b79b-103">**记录可能尚未在 Internet 上进行更新。**</span><span class="sxs-lookup"><span data-stu-id="9b79b-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="9b79b-104">通常只需几分钟，我们才能看到新记录，但偶尔可能需要几个小时的时间。</span><span class="sxs-lookup"><span data-stu-id="9b79b-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="9b79b-105">如果你已等待长时间，请仔细检查你是否已将确切的值复制并粘贴到 DNS 主机上的 TXT 验证记录中。</span><span class="sxs-lookup"><span data-stu-id="9b79b-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="9b79b-106">一个常见的问题是未包含记录的 "MS=" 部分。</span><span class="sxs-lookup"><span data-stu-id="9b79b-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="9b79b-107">我们也需要的！</span><span class="sxs-lookup"><span data-stu-id="9b79b-107">We need that too!</span></span>

- <span data-ttu-id="9b79b-108">在一些 DNS 主机上，你需要采取额外步骤来保存区域文件（存储 DNS记录的地方），以便它将通过 Internet 更新。</span><span class="sxs-lookup"><span data-stu-id="9b79b-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="9b79b-109">请确保您已保存所做的更改，以便 Microsoft 可以查看并验证记录。</span><span class="sxs-lookup"><span data-stu-id="9b79b-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
