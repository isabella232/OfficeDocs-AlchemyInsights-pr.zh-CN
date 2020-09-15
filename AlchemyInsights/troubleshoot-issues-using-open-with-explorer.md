---
title: 使用 "使用资源管理器打开" 解决问题
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659048"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="3711d-102">使用 "使用资源管理器打开" 解决问题</span><span class="sxs-lookup"><span data-stu-id="3711d-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="3711d-103">修复了使用 " **使用资源管理器打开** " 命令在 SharePoint 或 OneDrive 中打开文档库时遇到的常见问题：</span><span class="sxs-lookup"><span data-stu-id="3711d-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="3711d-104">使用 Internet Explorer 10 或 Internet Explorer 11。</span><span class="sxs-lookup"><span data-stu-id="3711d-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="3711d-105">**打开方式浏览器** 与 Microsoft Edge、Google Chrome、Firefox 和其他 Microsoft Edge 不兼容。</span><span class="sxs-lookup"><span data-stu-id="3711d-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="3711d-106">在除 Internet Explorer 之外的所有浏览器中禁用了 "**使用资源管理器打开**"。</span><span class="sxs-lookup"><span data-stu-id="3711d-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="3711d-107">在 SharePoint 库的新式体验中不提供 "**使用资源管理器打开**"。</span><span class="sxs-lookup"><span data-stu-id="3711d-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="3711d-108">改 **为使用文件资源管理器中的视图** 。</span><span class="sxs-lookup"><span data-stu-id="3711d-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="3711d-109">**View options** \> **在文件资源管理器中选择 "查看选项视图"**。</span><span class="sxs-lookup"><span data-stu-id="3711d-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="3711d-110">文件资源管理器中的视图与 Microsoft Edge、Google Chrome、Firefox 和其他项不兼容。</span><span class="sxs-lookup"><span data-stu-id="3711d-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="3711d-111">"**文件资源管理器**" 中的视图仅在 Internet Explorer 中可用。</span><span class="sxs-lookup"><span data-stu-id="3711d-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="3711d-112">请确保 WebClient 服务正在运行。</span><span class="sxs-lookup"><span data-stu-id="3711d-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="3711d-113">在 Windows 搜索框中，键入 "运行"，选择 "运行桌面应用"，键入 services.msc，然后按 Enter。</span><span class="sxs-lookup"><span data-stu-id="3711d-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="3711d-114">向下滚动到 WebClient 服务，并确保 " **状态** " 列显示 "正在运行"。</span><span class="sxs-lookup"><span data-stu-id="3711d-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="3711d-115">如果不是，请双击该服务，单击 " **开始**"，然后单击 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="3711d-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="3711d-116"> (您可能需要先通过在 "**启动类型**" 框中选择 "**手动**" 或 "**自动**" 来启用服务。 ) </span><span class="sxs-lookup"><span data-stu-id="3711d-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="3711d-117">如果需要复制或移动多个文件和文件夹一次，则在文件资源管理器中打开库非常方便，但如果要定期在库中工作，则建议将其同步。</span><span class="sxs-lookup"><span data-stu-id="3711d-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="3711d-118">要解决在文件资源管理器中打开的问题，请参阅 [在资源管理器中打开](https://go.microsoft.com/fwlink/?linkid=871665)。</span><span class="sxs-lookup"><span data-stu-id="3711d-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="3711d-119">有关设置同步的信息，请参阅 [Sync SharePoint files with the New OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666)。</span><span class="sxs-lookup"><span data-stu-id="3711d-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="3711d-120">有关详细信息，请参阅文章 [如何使用 "使用资源管理器打开" 命令来解决 SharePoint Online 中的问题](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) 。</span><span class="sxs-lookup"><span data-stu-id="3711d-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

