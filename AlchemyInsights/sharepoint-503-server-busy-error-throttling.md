---
title: SharePoint Online 限制
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 2aca55ac2fefbb2035140a759a77730dc905a4e9
ms.sourcegitcommit: 926e4ab6aa64ddc7a244de633421eb2b817541f2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2020
ms.locfileid: "42958708"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="419fa-102">SharePoint Online 限制</span><span class="sxs-lookup"><span data-stu-id="419fa-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="419fa-103">**重要说明**：在这些前所未有的时间内，我们将采取措施来确保 sharepoint Online 和 OneDrive 服务保持高可用性-有关详细信息，请参阅[Sharepoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)。</span><span class="sxs-lookup"><span data-stu-id="419fa-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="419fa-104">**503服务器忙碌错误**</span><span class="sxs-lookup"><span data-stu-id="419fa-104">**503 server is busy error**</span></span>

<span data-ttu-id="419fa-105">尝试导航到 SharePoint 或 OneDrive 网站时，用户可能会收到 "503 服务器占线" 错误。</span><span class="sxs-lookup"><span data-stu-id="419fa-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="419fa-106">此错误可能是由 SharePoint 服务中的限制导致的。</span><span class="sxs-lookup"><span data-stu-id="419fa-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="419fa-107">SharePoint Online 使用限制来维护 SharePoint Online 服务的最佳性能和可靠性。</span><span class="sxs-lookup"><span data-stu-id="419fa-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="419fa-108">限制会限制用户操作或并发调用数量（通过脚本或代码），以防止资源的过度使用。</span><span class="sxs-lookup"><span data-stu-id="419fa-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="419fa-109">有关限制的详细信息，请参阅[避免在 SharePoint Online 中受到限制或被阻止](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)。</span><span class="sxs-lookup"><span data-stu-id="419fa-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="419fa-110">如果您认为此错误与限制无关，可以通过导航到[消息中心](https://portal.office.com/adminportal/home#/MessageCenter)来检查租户上是否有活动的维护正在发生。</span><span class="sxs-lookup"><span data-stu-id="419fa-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="419fa-111">最后，请确保访问 "[服务运行状况](https://portal.office.com/adminportal/home#/servicehealth)" 页，以检查可能发生的任何咨询/事件。</span><span class="sxs-lookup"><span data-stu-id="419fa-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

