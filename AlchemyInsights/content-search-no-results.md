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
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516769"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="a8516-102">内容搜索/导出没有结果</span><span class="sxs-lookup"><span data-stu-id="a8516-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="a8516-103">不返回任何数据的内容搜索/导出的问题可能是由于特定管理员设置的某些合规性安全筛选器而不是将其与所有管理员通信。</span><span class="sxs-lookup"><span data-stu-id="a8516-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="a8516-104">若要解决此问题, 请检查是否存在可能导致此问题的合规性安全筛选器:</span><span class="sxs-lookup"><span data-stu-id="a8516-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="a8516-105">连接到安全与合规中心 Powershell</span><span class="sxs-lookup"><span data-stu-id="a8516-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="a8516-106">运行以下 commandlet:</span><span class="sxs-lookup"><span data-stu-id="a8516-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="a8516-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="a8516-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="a8516-108">New-compliancesecurityfilter-组织 $org</span><span class="sxs-lookup"><span data-stu-id="a8516-108">Get-ComplianceSecurityFilter -Organization $org</span></span>