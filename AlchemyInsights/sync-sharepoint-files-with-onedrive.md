---
title: 解答 SharePoint Online 中的“使用资源管理器打开”问题
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 13149d288336b487441c66521b32406e408911fd
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2019
ms.locfileid: "35803028"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="3483c-102">解答 SharePoint Online 中的“使用资源管理器打开”问题</span><span class="sxs-lookup"><span data-stu-id="3483c-102">Troubleshoot “Open with Explorer” issues in Sharepoint Online</span></span>

<span data-ttu-id="3483c-103">“使用资源管理器打开”命令将打开一个本地 Windows 资源管理器实例，其中显示托管 SharePoint 网站的服务器上的文件夹结构。</span><span class="sxs-lookup"><span data-stu-id="3483c-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="3483c-104">也就是说，我们建议[使用新版 OneDrive 同步客户端同步 SharePoint 文件](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>，该客户端提供[文件随选](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)，因为它提供了对文件的本地访问，并提供了最佳性能。</span><span class="sxs-lookup"><span data-stu-id="3483c-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="3483c-105">如果已选择使用资源管理器视图而不是使用新版 OneDrive 同步客户端，请确保遵循下文中所述的步骤和最佳做法：</span><span class="sxs-lookup"><span data-stu-id="3483c-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="3483c-106">如何使用“使用资源管理器打开”命令对 SharePoint Online 中的问题进行故障排除</span><span class="sxs-lookup"><span data-stu-id="3483c-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="3483c-107">通过“使用资源管理器打开”命令来复制或移动库文件</span><span class="sxs-lookup"><span data-stu-id="3483c-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> [!Note]  
> <span data-ttu-id="3483c-108">新的库体验中未显示“**使用资源管理器打**”按钮。</span><span class="sxs-lookup"><span data-stu-id="3483c-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="3483c-109">选择右上角的“**查看**”下拉菜单（下拉菜单的名称随当前视图的更改而变化），然后选择“**在文件资源管理器中查看**”。</span><span class="sxs-lookup"><span data-stu-id="3483c-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>

 ><span data-ttu-id="3483c-110">SharePoint 使用资源管理器打开时使用 ActiveX 控件，此仅在 Internet Explorer 10 或 11 中受支持。</span><span class="sxs-lookup"><span data-stu-id="3483c-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="3483c-111">“使用资源管理器打开”在使用 Microsoft Edge、Google Chrome、Mozilla Firefox 浏览器的 Windows 中或在 Mac 平台上不起作用。</span><span class="sxs-lookup"><span data-stu-id="3483c-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="3483c-112">由于这一原因, 资源管理器视图选项可能灰显。</span><span class="sxs-lookup"><span data-stu-id="3483c-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

> - <span data-ttu-id="3483c-113">[为什么 SharePoint 功能区按钮不可用或灰显](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca)。</span><span class="sxs-lookup"><span data-stu-id="3483c-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

