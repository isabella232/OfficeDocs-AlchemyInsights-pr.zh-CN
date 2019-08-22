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
ms.openlocfilehash: 1ef60017f1ea656296bc7b2aa3bc5365646f11f3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527585"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="e84be-102">启用邮箱审核</span><span class="sxs-lookup"><span data-stu-id="e84be-102">Enable mailbox auditing</span></span>

<span data-ttu-id="e84be-103">若要为单个用户或整个组织启用邮箱审核, 必须从远程 Power Shell 运行以下 cmdlet:</span><span class="sxs-lookup"><span data-stu-id="e84be-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="e84be-104">**单个用户**</span><span class="sxs-lookup"><span data-stu-id="e84be-104">**Single User**</span></span>
  
<span data-ttu-id="e84be-105">Set-邮箱-Identity "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="e84be-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="e84be-106">**组织**</span><span class="sxs-lookup"><span data-stu-id="e84be-106">**Organization**</span></span>
  
<span data-ttu-id="e84be-107">ResultSize 无限制-筛选器 {RecipientTypeDetails-eq "UserMailbox"} |Set-邮箱-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="e84be-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="e84be-108">了解更多</span><span class="sxs-lookup"><span data-stu-id="e84be-108">Learn more</span></span>](https://support.office.com/article/aaca8987-5b62-458b-9882-c28476a66918)
  

