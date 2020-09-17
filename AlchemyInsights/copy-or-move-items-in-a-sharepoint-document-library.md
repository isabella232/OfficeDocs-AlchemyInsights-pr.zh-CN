---
title: 复制或移动 SharePoint 文档库中的项
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
ms.custom:
- "454"
- "5300013"
ms.assetid: 592f502a-493f-4bf4-adc3-5bc8aea87bb5
ms.openlocfilehash: d7aa865a6b3db0871a57313dd7d6f5b0213ca0e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807109"
---
# <a name="copy-or-move-items-in-a-sharepoint-document-library"></a><span data-ttu-id="cff75-102">复制或移动 SharePoint 文档库中的项</span><span class="sxs-lookup"><span data-stu-id="cff75-102">Copy or move items in a SharePoint document library</span></span>

<span data-ttu-id="cff75-103">您可以复制并移动到文档库中的不同位置的文件、文件夹和链接。</span><span class="sxs-lookup"><span data-stu-id="cff75-103">You can copy and move files, folders, and links to different locations within a document library.</span></span> <span data-ttu-id="cff75-104">您还可以跨网站复制项目。</span><span class="sxs-lookup"><span data-stu-id="cff75-104">You can also copy items across sites.</span></span> 
  
1. <span data-ttu-id="cff75-105">在浏览器中，浏览到要移动的文件、文件夹或链接，然后单击 " **复制到** " 或 " **移动到**"。</span><span class="sxs-lookup"><span data-stu-id="cff75-105">In a browser, browse to the files, folders, or links you want to move, and then click **Copy to** or **Move to**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="cff75-106">如果使用的是 SharePoint Online 的经典体验，"**复制到**" 和 "**移动到**" 将不可用。</span><span class="sxs-lookup"><span data-stu-id="cff75-106">**Copy to** and **Move to** aren't available if you're using the classic experience of SharePoint Online.</span></span>
  
2. <span data-ttu-id="cff75-107">在 " **选择目标**" 下，选择要将项目复制或移动到的位置，或单击 " **浏览网站** " 以查看完整的网站列表。</span><span class="sxs-lookup"><span data-stu-id="cff75-107">Under **Choose a destination**, select the location to which you want to copy or move the items or click **Browse sites** to see the full list of sites.</span></span>

    > [!NOTE]
    > <span data-ttu-id="cff75-108">如果在复制项目时未看到列出的其他网站，则尚未配置跨网站复制。</span><span class="sxs-lookup"><span data-stu-id="cff75-108">If you don't see other sites listed when you copy items, copying across sites hasn't been configured.</span></span> <span data-ttu-id="cff75-109">若要启用它，请转到 SharePoint 管理中心的 "设置" 页，然后单击 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="cff75-109">To enable it, go to the settings page of the SharePoint admin center and click **OK**.</span></span>
  
    <span data-ttu-id="cff75-110">若要创建新文件夹，请选择文件夹层次结构中的位置，单击 " **新建文件夹**"，为该文件夹输入一个名称，然后单击复选标记以保存该名称。</span><span class="sxs-lookup"><span data-stu-id="cff75-110">To create a new folder, select a location in the folder hierarchy, click **New folder**, enter a name for the folder, and click the check mark to save the name.</span></span>

3. <span data-ttu-id="cff75-111">单击 " **复制到此处** " 或 "移动到 **此处**"。</span><span class="sxs-lookup"><span data-stu-id="cff75-111">Click **Copy here** or **Move here**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="cff75-112">一次最多可以复制 500 MB 的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="cff75-112">You can copy up to 500 MB of files and folders at one time.</span></span> <span data-ttu-id="cff75-113">> 复制具有版本历史记录的文档时，仅复制最新版本。</span><span class="sxs-lookup"><span data-stu-id="cff75-113">>  When you copy documents that have version history, only the latest version is copied.</span></span> <span data-ttu-id="cff75-114">移动文档时，也会移动文档的历史记录。</span><span class="sxs-lookup"><span data-stu-id="cff75-114">When you move documents, their history is also moved.</span></span>
  
 <span data-ttu-id="cff75-115">当文件移动时，它仍将出现在源目录中，直到它完全移动到目标，然后才会被删除。</span><span class="sxs-lookup"><span data-stu-id="cff75-115">When a file is moving, it will still appear in the source directory until its fully moved to the destination, and then it will be deleted.</span></span> <span data-ttu-id="cff75-116">移动完成后，文件将保留在源网站回收站中，并遵循正常的回收计划，除非用户从回收站中恢复。</span><span class="sxs-lookup"><span data-stu-id="cff75-116">The file will remain in the source sites recycle bin after the move is complete and be subject to the normal recycle schedule unless a user recovers it from the recycle bin.</span></span>

<span data-ttu-id="cff75-117">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="cff75-117">For more information, see:</span></span>

 - <span data-ttu-id="cff75-118">[在 SharePoint 中移动或复制文件](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office 支持文章) </span><span class="sxs-lookup"><span data-stu-id="cff75-118">[Move or copy files in SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office support article)</span></span>
 - <span data-ttu-id="cff75-119">[从任何文件夹移动文件](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft 技术社区博客文章) </span><span class="sxs-lookup"><span data-stu-id="cff75-119">[Move files from any folder](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community blog article)</span></span>  