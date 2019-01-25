---
title: 使用资源管理器打开操作不起作用
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29458945"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="74c7f-102">使用资源管理器打开不工作</span><span class="sxs-lookup"><span data-stu-id="74c7f-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="74c7f-p101">如果**使用资源管理器中打开**或**在文件资源管理器视图**不起作用确保 WebClient 服务设置为**运行**通过执行以下步骤。例如，可能需要很长时间才能服务未运行时打开的 SharePoint 或 OneDrive 库。</span><span class="sxs-lookup"><span data-stu-id="74c7f-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="74c7f-105">在 Windows 搜索框中，键入运行，选择运行桌面应用程序，键入 services.msc，然后选择**enter 键**。</span><span class="sxs-lookup"><span data-stu-id="74c7f-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="74c7f-p102">向下滚动到 WebClient 服务，并检查**状态**列。如果 WebClient 服务状态不是**运行**，双击的服务，单击**开始**，然后单击**确定**。如果需要通过在**启动类型**框中选择**手动**或**自动**，启用该服务。</span><span class="sxs-lookup"><span data-stu-id="74c7f-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="74c7f-p103">若要解决在文件资源管理器中打开的问题，请参阅[在资源管理器中打开](https://go.microsoft.com/fwlink/?linkid=871665)。浏览更好的替代项为同步：[同步 SharePoint 文件使用新的 OneDrive 同步客户端](https://go.microsoft.com/fwlink/?linkid=871666)。</span><span class="sxs-lookup"><span data-stu-id="74c7f-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

