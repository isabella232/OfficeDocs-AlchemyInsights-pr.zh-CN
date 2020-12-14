---
title: 内容搜索/导出期间未返回任何结果
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/14/2020
ms.locfileid: "49666638"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="28322-102">内容搜索/导出期间未返回任何结果</span><span class="sxs-lookup"><span data-stu-id="28322-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="28322-103">如果遇到以下电子数据展示方案的问题：</span><span class="sxs-lookup"><span data-stu-id="28322-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="28322-104">内容搜索/导出不会返回任何数据或意外数据</span><span class="sxs-lookup"><span data-stu-id="28322-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="28322-105">电子数据展示搜索或导出失败</span><span class="sxs-lookup"><span data-stu-id="28322-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="28322-106">这可能是由特定管理员设置且未传达给所有管理员的某些合规性安全筛选器导致的。</span><span class="sxs-lookup"><span data-stu-id="28322-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="28322-107">若要解决此问题，请检查是否有可能导致这些问题的合规性安全筛选器：</span><span class="sxs-lookup"><span data-stu-id="28322-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="28322-108">连接到安全与合规中心 Powershell</span><span class="sxs-lookup"><span data-stu-id="28322-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="28322-109">运行以下命令let：</span><span class="sxs-lookup"><span data-stu-id="28322-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="28322-110">有关合规性安全筛选器的其他信息，请参阅 [内容搜索的权限筛选](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="28322-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
