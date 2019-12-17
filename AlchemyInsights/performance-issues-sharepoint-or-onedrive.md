---
title: 性能问题-SharePoint 或 OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068382"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="48f9a-102">SharePoint 或 OneDrive 速度慢、不可访问或对多个用户不可用</span><span class="sxs-lookup"><span data-stu-id="48f9a-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="48f9a-103">SharePoint 或 OneDrive 的速度可能很慢、不可访问或不可用，或者因以下几个原因而显示服务不可用或503错误：</span><span class="sxs-lookup"><span data-stu-id="48f9a-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="48f9a-104">如果您的 SharePoint 或 OneDrive 网站的多个用户的速度较慢或延迟，则在访问 SharePoint 网站或 OneDrive 内容时，用户可能会遇到间歇延迟或导航错误的临时服务问题。</span><span class="sxs-lookup"><span data-stu-id="48f9a-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="48f9a-105">检查[服务运行状况仪表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)以查看您的组织是否受到影响。</span><span class="sxs-lookup"><span data-stu-id="48f9a-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="48f9a-106">尝试导航到 SharePoint 或 OneDrive 网站时，用户可能会收到 " *503 服务器占线*" 错误。</span><span class="sxs-lookup"><span data-stu-id="48f9a-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="48f9a-107">此错误可能是由 SharePoint 服务中的限制导致的。</span><span class="sxs-lookup"><span data-stu-id="48f9a-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="48f9a-108">SharePoint Online 使用限制来维护 SharePoint Online 服务的最佳性能和可靠性。</span><span class="sxs-lookup"><span data-stu-id="48f9a-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="48f9a-109">限制会限制用户操作或并发调用数量（通过脚本或代码），以防止资源的过度使用。</span><span class="sxs-lookup"><span data-stu-id="48f9a-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="48f9a-110">有关限制的详细信息，请参阅[避免在 SharePoint Online 中受到限制或被阻止](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)。</span><span class="sxs-lookup"><span data-stu-id="48f9a-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="48f9a-111">如果您在使用**经典**或**新式**SharePoint 网站或页面时遇到性能降低的情况，请使用[页面诊断工具](https://aka.ms/perftool)来分析页面。</span><span class="sxs-lookup"><span data-stu-id="48f9a-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="48f9a-112">如果仍遇到常规低性能，请查看本文底部的资源： [SharePoint Online 的性能优化简介](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="48f9a-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  