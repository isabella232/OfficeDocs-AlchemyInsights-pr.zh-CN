---
title: 解答 SharePoint Online 中的“使用资源管理器打开”问题
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6462"
- "9003546"
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: ea93bb6f3cbbc3424f5e006ffac482a7445c8164
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086038"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="e68d7-102">解答 SharePoint Online 中的“使用资源管理器打开”问题</span><span class="sxs-lookup"><span data-stu-id="e68d7-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="e68d7-103">请按照以下文章中的步骤和最佳做法进行操作：</span><span class="sxs-lookup"><span data-stu-id="e68d7-103">Follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="e68d7-104">如何使用“使用资源管理器打开”命令解决 SharePoint Online 中的问题</span><span class="sxs-lookup"><span data-stu-id="e68d7-104">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/troubleshoot/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)

- [<span data-ttu-id="e68d7-105">通过“使用资源管理器打开”命令来复制或移动库文件</span><span class="sxs-lookup"><span data-stu-id="e68d7-105">Copy or move library files by using Open with Explorer</span></span>](https://support.microsoft.com/office/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2?ui=en-us&rs=en-us&ad=us)

> [!NOTE]
- <span data-ttu-id="e68d7-106">我们建议[使用新版 OneDrive 同步客户端同步 SharePoint 文件](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us)，该客户端提供[文件随选](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us)，因为同步授予了对文件的本地访问权限，并提供了最佳性能。</span><span class="sxs-lookup"><span data-stu-id="e68d7-106">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us) which provides [Files On-Demand](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us) because the synchronization grants local access to your files and offers the best performance.</span></span>

- <span data-ttu-id="e68d7-107">仅在 Internet Explorer 11 中支持“**使用资源管理器打开**”。</span><span class="sxs-lookup"><span data-stu-id="e68d7-107">**Open with Explorer** is only supported in Internet Explorer 11.</span></span> <span data-ttu-id="e68d7-108">有关详细信息，请参阅 [终止对使用 Microsoft 365 应用版的 IE11 的支持](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy)。</span><span class="sxs-lookup"><span data-stu-id="e68d7-108">For more information, see [end of support for IE11 with Microsoft 365 Apps](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy)).</span></span> <span data-ttu-id="e68d7-109">“**使用资源管理器打开**”在使用 Microsoft Edge、Google Chrome、Mozilla Firefox 浏览器的 Windows 中或在 Mac 平台上不起作用。</span><span class="sxs-lookup"><span data-stu-id="e68d7-109">**Open with Explorer** doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="e68d7-110">由于这一原因, “**资源管理器视图**”选项可能灰显。</span><span class="sxs-lookup"><span data-stu-id="e68d7-110">Due to this reason, the **Explorer View** option may be grayed out.</span></span> 

- <span data-ttu-id="e68d7-111">新的库体验中未显示“**使用资源管理器打开**”按钮。</span><span class="sxs-lookup"><span data-stu-id="e68d7-111">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="e68d7-112">选择右上角的“**查看**”下拉菜单（下拉菜单的名称随当前视图的更改而变化），然后选择“**在文件资源管理器中查看**”。</span><span class="sxs-lookup"><span data-stu-id="e68d7-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>

