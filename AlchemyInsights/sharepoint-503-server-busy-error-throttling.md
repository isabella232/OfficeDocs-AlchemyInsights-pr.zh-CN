---
title: SharePoint Online 限制
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 21d0f8d0118d92562b425921742513157563b5fb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47773837"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="423f1-102">SharePoint Online 限制</span><span class="sxs-lookup"><span data-stu-id="423f1-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="423f1-103">**重要信息：** 在这段前所未有的时期，我们正在采取措施确保 SharePoint Online 和 OneDrive 服务高度可用，请访问 [SharePoint Online 临时功能调整](https://aka.ms/ODSPAdjustments)，获取详细信息。</span><span class="sxs-lookup"><span data-stu-id="423f1-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="423f1-104">**503服务器忙碌错误**</span><span class="sxs-lookup"><span data-stu-id="423f1-104">**503 server is busy error**</span></span>

<span data-ttu-id="423f1-105">尝试导航到 SharePoint 或 OneDrive 网站时，用户可能会收到 "503 服务器占线" 错误。</span><span class="sxs-lookup"><span data-stu-id="423f1-105">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="423f1-106">此错误可能是由 SharePoint 服务中的限制导致的。</span><span class="sxs-lookup"><span data-stu-id="423f1-106">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="423f1-107">SharePoint Online 使用限制来维护 SharePoint Online 服务的最佳性能和可靠性。</span><span class="sxs-lookup"><span data-stu-id="423f1-107">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="423f1-108">限制（通过脚本或代码）对用户操作数量或并发性调用进行限制，以阻止资源的过度使用。</span><span class="sxs-lookup"><span data-stu-id="423f1-108">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="423f1-109">有关限制的详细信息，请参阅 [避免在 SharePoint Online 中受到限制或被阻止](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)。</span><span class="sxs-lookup"><span data-stu-id="423f1-109">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="423f1-110">如果您认为此错误与限制无关，可以通过导航到 [消息中心](https://portal.office.com/adminportal/home#/MessageCenter)来检查租户上是否有活动的维护正在发生。</span><span class="sxs-lookup"><span data-stu-id="423f1-110">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="423f1-111">最后，请确保访问 " [服务运行状况](https://portal.office.com/adminportal/home#/servicehealth) " 页，以检查可能发生的任何咨询/事件。</span><span class="sxs-lookup"><span data-stu-id="423f1-111">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

