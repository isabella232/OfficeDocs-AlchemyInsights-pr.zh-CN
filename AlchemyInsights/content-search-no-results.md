---
title: 内容搜索无结果
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800202"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="55b22-102">内容搜索/导出没有结果</span><span class="sxs-lookup"><span data-stu-id="55b22-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="55b22-103">不返回任何数据的内容搜索/导出的问题可能是由于特定管理员设置的某些合规性安全筛选器而不是将其与所有管理员通信。</span><span class="sxs-lookup"><span data-stu-id="55b22-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="55b22-104">若要解决此问题, 请检查是否存在可能导致此问题的合规性安全筛选器:</span><span class="sxs-lookup"><span data-stu-id="55b22-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="55b22-105">连接到安全与合规中心 Powershell</span><span class="sxs-lookup"><span data-stu-id="55b22-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="55b22-106">运行以下 commandlet:</span><span class="sxs-lookup"><span data-stu-id="55b22-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="55b22-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="55b22-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="55b22-108">New-compliancesecurityfilter-组织 $org</span><span class="sxs-lookup"><span data-stu-id="55b22-108">Get-ComplianceSecurityFilter -Organization $org</span></span>