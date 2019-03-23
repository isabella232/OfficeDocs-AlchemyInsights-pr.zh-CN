---
title: 启用邮箱审核
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 19997b0a-394f-4943-8908-c601696a332c
ms.openlocfilehash: 81041685cf383a231a9a9739d6daffd6039b4602
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2019
ms.locfileid: "30757808"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="219b7-102">启用邮箱审核</span><span class="sxs-lookup"><span data-stu-id="219b7-102">Enable mailbox auditing</span></span>

<span data-ttu-id="219b7-103">若要为单个用户或整个组织启用邮箱审核, 必须从远程 Power Shell 运行以下 cmdlet:</span><span class="sxs-lookup"><span data-stu-id="219b7-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="219b7-104">**单个用户**</span><span class="sxs-lookup"><span data-stu-id="219b7-104">**Single User**</span></span>
  
<span data-ttu-id="219b7-105">Set-邮箱-Identity "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="219b7-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="219b7-106">**组织**</span><span class="sxs-lookup"><span data-stu-id="219b7-106">**Organization**</span></span>
  
<span data-ttu-id="219b7-107">ResultSize 无限制-筛选器 {RecipientTypeDetails-eq "UserMailbox"} |Set-邮箱-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="219b7-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="219b7-108">了解更多</span><span class="sxs-lookup"><span data-stu-id="219b7-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

