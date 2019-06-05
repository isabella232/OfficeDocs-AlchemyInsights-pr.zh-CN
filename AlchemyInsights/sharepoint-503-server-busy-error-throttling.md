---
title: SharePoint Online 限制
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 620a1094c1926b2c095c057a1791aaed8383afb3
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716917"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="5ed96-102">SharePoint Online 限制</span><span class="sxs-lookup"><span data-stu-id="5ed96-102">SharePoint Online Throttling</span></span>

<p><span data-ttu-id="5ed96-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">尝试导航到 Sharepoint 或 OneDrive 网站时, 用户可能会收到 "503 服务器占线" 错误。</span></span><span class="sxs-lookup"><span data-stu-id="5ed96-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Users may receive a 503 server is busy error when attempting to navigate to Sharepoint or OneDrive sites. </span></span></span></p> <p><span data-ttu-id="5ed96-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">此错误可能是由 Sharepoint 服务中的限制导致的。SharePoint Online 使用限制来维护 SharePoint Online 服务的最佳性能和可靠性。限制限制用户操作或并发呼叫数 (按脚本或代码) 以防止过度使用资源。如果您确实遇到了限制, 则 99% 的时间是由于自定义代码而导致的。</span></span><span class="sxs-lookup"><span data-stu-id="5ed96-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">This error can be caused by throttling within the Sharepoint service. SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service. Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources. If you do get throttled, 99% of the time it is because of custom code.</span></span></span></p> <p><span data-ttu-id="5ed96-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">有关限制的详细信息, 请参阅<a href="https://docs.microsoft.com/en-us/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online">避免在 SharePoint Online 中受到限制或被阻止</a>。</span></span><span class="sxs-lookup"><span data-stu-id="5ed96-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">For more information on throttling see, <a href="https://docs.microsoft.com/en-us/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online">Avoid getting throttled or blocked in SharePoint Online</a>.</span></span></span></p> <p><span data-ttu-id="5ed96-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">如果您认为此错误与限制无关, 可以通过导航到<a href="https://portal.office.com/adminportal/home#/MessageCenter">消息中心</a>来检查租户上是否有活动的维护正在发生。最后, 请确保访问 "<a href="https://portal.office.com/adminportal/home#/servicehealth">服务运行状况</a>" 页, 以检查可能发生的任何咨询/事件。</span></span><span class="sxs-lookup"><span data-stu-id="5ed96-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the <a href="https://portal.office.com/adminportal/home#/MessageCenter">Message center</a>. Finally , ensure you visit the <a href="https://portal.office.com/adminportal/home#/servicehealth">Service Health</a> page to check for any advisories/incidents that may be occurring.</span></span></span></p> <p>&nbsp;</p>


