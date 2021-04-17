---
title: 内容搜索无结果
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816838"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="d1daa-102">没有来自内容搜索/导出的结果</span><span class="sxs-lookup"><span data-stu-id="d1daa-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="d1daa-103">内容搜索/导出未返回任何数据的问题可能是由于特定管理员设置的特定合规性安全筛选器，未将它传达到所有管理员。</span><span class="sxs-lookup"><span data-stu-id="d1daa-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="d1daa-104">若要解决此问题，请检查是否有可能导致此情况出现的任何合规性安全筛选器：</span><span class="sxs-lookup"><span data-stu-id="d1daa-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="d1daa-105">连接到安全与合规中心 Powershell</span><span class="sxs-lookup"><span data-stu-id="d1daa-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="d1daa-106">运行以下命令let：</span><span class="sxs-lookup"><span data-stu-id="d1daa-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="d1daa-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="d1daa-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="d1daa-108">Get-ComplianceSecurityFilter -Organization $org</span><span class="sxs-lookup"><span data-stu-id="d1daa-108">Get-ComplianceSecurityFilter -Organization $org</span></span>