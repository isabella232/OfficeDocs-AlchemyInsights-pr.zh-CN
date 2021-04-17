---
title: 使用基于 Chromium 浏览器的 Microsoft Edge 进行 Ediscovery 导出
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
- "3473"
- "3100022"
ms.openlocfilehash: 7ee724e5109effce8883be50e360948313c84b34
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834361"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a><span data-ttu-id="2a05f-102">使用基于 Chromium 浏览器的 Microsoft Edge 进行 Ediscovery 导出</span><span class="sxs-lookup"><span data-stu-id="2a05f-102">Using Microsoft Edge based on Chromium browsers for Ediscovery export</span></span>

<span data-ttu-id="2a05f-103">由于最近的更改，默认情况下，Microsoft Edge ClickOnce不再启用支持。</span><span class="sxs-lookup"><span data-stu-id="2a05f-103">Due to a recent change, Microsoft Edge browsers will no longer have ClickOnce support enabled by default.</span></span> <span data-ttu-id="2a05f-104">若要继续使用 Microsoft 365 电子数据展示导出工具，你将需要使用 Microsoft Internet Explorer或在 Microsoft Edge ClickOnce支持。</span><span class="sxs-lookup"><span data-stu-id="2a05f-104">To continue using the Microsoft 365 eDiscovery Export Tool, you will either need to use Microsoft Internet Explorer or enable ClickOnce Support in Microsoft Edge.</span></span> 

<span data-ttu-id="2a05f-105">若要启用ClickOnce Chromium 在 Microsoft Edge 中启用支持：</span><span class="sxs-lookup"><span data-stu-id="2a05f-105">To enable ClickOnce Support in Microsoft Edge based on Chromium:</span></span> 
1. <span data-ttu-id="2a05f-106">在 Microsoft Edge 浏览器中，访问 edge://flags/#edge-click-once。</span><span class="sxs-lookup"><span data-stu-id="2a05f-106">In your Microsoft Edge browser, visit edge://flags/#edge-click-once.</span></span>
2. <span data-ttu-id="2a05f-107">对于 ClickOnce 支持选项，将值从“**默认**”或“**已禁用**”更改为“**已启用**”。</span><span class="sxs-lookup"><span data-stu-id="2a05f-107">For the ClickOnce Support option, change the value from **Default** or **Disabled** to **Enabled**.</span></span> 
3. <span data-ttu-id="2a05f-108">在浏览器窗口底部，选择"重新启动 **"。**</span><span class="sxs-lookup"><span data-stu-id="2a05f-108">At the bottom of the browser window, select **Restart**.</span></span> <br>
 <span data-ttu-id="2a05f-109">更改将在重启 Microsoft Edge 后生效。</span><span class="sxs-lookup"><span data-stu-id="2a05f-109">The change will take effect after restarting Microsoft Edge.</span></span> 

<span data-ttu-id="2a05f-110">有关这一点以及安装导出工具的步骤的信息，请参阅： [ 导出内容搜索结果](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)。</span><span class="sxs-lookup"><span data-stu-id="2a05f-110">For information on this and steps for installing the  export tool, see: [ Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>