---
title: 电子数据展示导出工具
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277921"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="e3d90-102">无法安装或运行电子数据展示导出工具？</span><span class="sxs-lookup"><span data-stu-id="e3d90-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="e3d90-103">如果无法安装或运行电子数据展示导出工具以下载搜索结果，请检查以下各项：</span><span class="sxs-lookup"><span data-stu-id="e3d90-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="e3d90-104">您正在使用的计算机满足以下先决条件：</span><span class="sxs-lookup"><span data-stu-id="e3d90-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="e3d90-105">32 位或 64 位版本的 Windows 7 和更高版本</span><span class="sxs-lookup"><span data-stu-id="e3d90-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="e3d90-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="e3d90-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="e3d90-107">支持的浏览器：</span><span class="sxs-lookup"><span data-stu-id="e3d90-107">A supported browser:</span></span>

  - <span data-ttu-id="e3d90-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="e3d90-108">Microsoft Edge</span></span>

    <span data-ttu-id="e3d90-109">或</span><span class="sxs-lookup"><span data-stu-id="e3d90-109">Or</span></span>

  - <span data-ttu-id="e3d90-110">Internet Explorer 10 和更高版本</span><span class="sxs-lookup"><span data-stu-id="e3d90-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="e3d90-111">其他浏览器（如 Google Chrome 和 Mozilla Firefox）不受支持。</span><span class="sxs-lookup"><span data-stu-id="e3d90-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="e3d90-112">您的组织可以连接到 Azure 中的终结点，即\*\* \* blob.core.windows.net\*\* (通配符代表导出作业) 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e3d90-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="e3d90-113">你已在 Microsoft 365 安全合规中心中分配了导出角色 &amp; 。</span><span class="sxs-lookup"><span data-stu-id="e3d90-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="e3d90-114">默认情况下，此角色仅分配给电子数据展示管理器角色组。</span><span class="sxs-lookup"><span data-stu-id="e3d90-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="e3d90-115">请参阅 [分配电子数据展示权限](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)。</span><span class="sxs-lookup"><span data-stu-id="e3d90-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="e3d90-116">有关详细信息，请参阅 [导出内容搜索结果](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)。</span><span class="sxs-lookup"><span data-stu-id="e3d90-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="e3d90-117">如果要导出超过10万个以上的邮箱，则需要使用以下 Powershell 下载导出结果：  [导出超过10个邮箱的结果](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)。</span><span class="sxs-lookup"><span data-stu-id="e3d90-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>