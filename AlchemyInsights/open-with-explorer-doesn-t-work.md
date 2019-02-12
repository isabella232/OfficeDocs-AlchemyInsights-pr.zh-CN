---
title: 使用资源管理器打开操作不起作用
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: f788c3c626cdeb19970edb59563c59eea60e2992
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906794"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="1913c-102">使用资源管理器打开不工作</span><span class="sxs-lookup"><span data-stu-id="1913c-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="1913c-p101">如果**使用资源管理器中打开**或**在文件资源管理器视图**不起作用确保 WebClient 服务设置为**运行**通过执行以下步骤。例如，可能需要很长时间才能服务未运行时打开的 SharePoint 或 OneDrive 库。</span><span class="sxs-lookup"><span data-stu-id="1913c-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="1913c-105">在 Windows 搜索框中，键入运行，选择运行桌面应用程序，键入 services.msc，然后选择**enter 键**。</span><span class="sxs-lookup"><span data-stu-id="1913c-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="1913c-p102">向下滚动到 WebClient 服务，并检查**状态**列。如果 WebClient 服务状态不是**运行**，双击的服务，单击**开始**，然后单击**确定**。如果需要通过在**启动类型**框中选择**手动**或**自动**，启用该服务。</span><span class="sxs-lookup"><span data-stu-id="1913c-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="1913c-p103">若要解决在文件资源管理器中打开的问题，请参阅[在资源管理器中打开](https://go.microsoft.com/fwlink/?linkid=871665)。浏览更好的替代项为同步：[同步 SharePoint 文件使用新的 OneDrive 同步客户端](https://go.microsoft.com/fwlink/?linkid=871666)。</span><span class="sxs-lookup"><span data-stu-id="1913c-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

