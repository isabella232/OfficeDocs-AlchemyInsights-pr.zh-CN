---
title: 使用资源管理器打开不起作用
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419853"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="9f877-102">使用资源管理器打开不起作用</span><span class="sxs-lookup"><span data-stu-id="9f877-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="9f877-103">如果**使用资源管理器打开**或**在文件资源管理器中查看**不起作用, 请按照下面的步骤操作, 以确保将 WebClient 服务设置为 "**正在运行**"。</span><span class="sxs-lookup"><span data-stu-id="9f877-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="9f877-104">例如, 当服务未运行时, 可能需要很长时间才能打开 SharePoint 或 OneDrive 库。</span><span class="sxs-lookup"><span data-stu-id="9f877-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="9f877-105">在 Windows 搜索框中, 键入 "运行", 选择 "运行桌面应用", 键入 "services.msc", 然后选择 "**输入**"。</span><span class="sxs-lookup"><span data-stu-id="9f877-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="9f877-106">向下滚动到 WebClient 服务并检查 "**状态**" 列。</span><span class="sxs-lookup"><span data-stu-id="9f877-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="9f877-107">如果 WebClient 服务状态未**运行**, 请双击该服务, 单击 "**开始**", 然后单击 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="9f877-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="9f877-108">如果需要, 可通过在 "**启动类型**" 框中选择 "**手动**" 或 "**自动**" 来启用服务。</span><span class="sxs-lookup"><span data-stu-id="9f877-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="9f877-109">要解决在文件资源管理器中打开的问题, 请参阅[在资源管理器中打开](https://go.microsoft.com/fwlink/?linkid=871665)。</span><span class="sxs-lookup"><span data-stu-id="9f877-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="9f877-110">浏览同步作为更好的替代方法:[使用新的 OneDrive 同步客户端同步 SharePoint 文件](https://go.microsoft.com/fwlink/?linkid=871666)。</span><span class="sxs-lookup"><span data-stu-id="9f877-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

