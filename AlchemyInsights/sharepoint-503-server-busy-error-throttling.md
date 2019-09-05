---
title: SharePoint Online 限制
ms.author: pebaum
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: d9e1400697b1e6435fea78703d2ecadc6733a57f
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751878"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="3b470-102">SharePoint Online 限制</span><span class="sxs-lookup"><span data-stu-id="3b470-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="3b470-103">尝试导航到 SharePoint 或 OneDrive 网站时，用户可能会收到 "503 服务器占线" 错误。</span><span class="sxs-lookup"><span data-stu-id="3b470-103">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="3b470-104">此错误可能是由 SharePoint 服务中的限制导致的。</span><span class="sxs-lookup"><span data-stu-id="3b470-104">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="3b470-105">SharePoint Online 使用限制来维护 SharePoint Online 服务的最佳性能和可靠性。</span><span class="sxs-lookup"><span data-stu-id="3b470-105">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="3b470-106">限制会限制用户操作或并发调用数量（通过脚本或代码），以防止资源的过度使用。</span><span class="sxs-lookup"><span data-stu-id="3b470-106">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="3b470-107">如果您被限制，99% 都是因为自定义代码。</span><span class="sxs-lookup"><span data-stu-id="3b470-107">If you do get throttled, 99% of the time it is because of custom code.</span></span>

<span data-ttu-id="3b470-108">有关限制的详细信息，请参阅[避免在 SharePoint Online 中受到限制或被阻止](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)。</span><span class="sxs-lookup"><span data-stu-id="3b470-108">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="3b470-109">如果您认为此错误与限制无关，可以通过导航到[消息中心](https://portal.office.com/adminportal/home#/MessageCenter)来检查租户上是否有活动的维护正在发生。</span><span class="sxs-lookup"><span data-stu-id="3b470-109">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="3b470-110">最后，请确保访问 "[服务运行状况](https://portal.office.com/adminportal/home#/servicehealth)" 页，以检查可能发生的任何咨询/事件。</span><span class="sxs-lookup"><span data-stu-id="3b470-110">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

