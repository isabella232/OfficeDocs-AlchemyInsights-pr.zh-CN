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
ms.openlocfilehash: 73517f46935a67a4a8a3e4770090ac897fe67979
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736243"
---
# <a name="enable-mailbox-auditing"></a><span data-ttu-id="ef64f-102">启用邮箱审核</span><span class="sxs-lookup"><span data-stu-id="ef64f-102">Enable mailbox auditing</span></span>

<span data-ttu-id="ef64f-103">若要为单个用户或整个组织启用邮箱审核，必须从远程 Power Shell 运行以下 cmdlet：</span><span class="sxs-lookup"><span data-stu-id="ef64f-103">To enable Mailbox Auditing for either a single user or an entire organization the following cmdlets must be run from Remote Power Shell:</span></span>
  
 <span data-ttu-id="ef64f-104">**单个用户**</span><span class="sxs-lookup"><span data-stu-id="ef64f-104">**Single User**</span></span>
  
<span data-ttu-id="ef64f-105">Set-邮箱-Identity "Jane Dow"-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="ef64f-105">Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true</span></span>
  
 <span data-ttu-id="ef64f-106">**组织**</span><span class="sxs-lookup"><span data-stu-id="ef64f-106">**Organization**</span></span>
  
<span data-ttu-id="ef64f-107">ResultSize 无限制-筛选器 {RecipientTypeDetails-eq "UserMailbox"} |Set-邮箱-AuditEnabled $true</span><span class="sxs-lookup"><span data-stu-id="ef64f-107">Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} | Set-Mailbox -AuditEnabled $true</span></span>
  
[<span data-ttu-id="ef64f-108">了解更多</span><span class="sxs-lookup"><span data-stu-id="ef64f-108">Learn more</span></span>](https://docs.microsoft.com/office365/securitycompliance/enable-mailbox-auditing)
  

