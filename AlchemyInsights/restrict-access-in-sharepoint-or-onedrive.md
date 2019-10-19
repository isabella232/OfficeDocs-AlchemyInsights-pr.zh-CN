---
title: 在 SharePoint 或 OneDrive 中限制访问权限
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551441"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="27598-102">在 SharePoint 或 OneDrive 中限制访问权限</span><span class="sxs-lookup"><span data-stu-id="27598-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="27598-103">在 SharePoint 和 OneDrive 中，通过仅向要访问的组或个人授予访问权限，可以限制对文件、文件夹和列表等项目的访问。</span><span class="sxs-lookup"><span data-stu-id="27598-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="27598-104">默认情况下，SharePoint 中的权限从层次结构中的较高版本继承。</span><span class="sxs-lookup"><span data-stu-id="27598-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="27598-105">因此，文件从文件夹继承其权限，这将从库继承其权限，这将从网站继承权限。</span><span class="sxs-lookup"><span data-stu-id="27598-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="27598-106">您可以在更高的级别（例如，通过共享整个网站）进行共享，如果您不想在网站上共享所有项目，则会中断继承。</span><span class="sxs-lookup"><span data-stu-id="27598-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="27598-107">但是，我们不建议这样做，因为这会使这些权限在将来保持更复杂和更容易混淆。</span><span class="sxs-lookup"><span data-stu-id="27598-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="27598-108">您可以改为执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="27598-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="27598-109">例如，如果您想要共享一个文件夹中除一个文件之外的所有内容，请将该文件移动到一个不共享的新位置。</span><span class="sxs-lookup"><span data-stu-id="27598-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="27598-110">如果文件夹中有两个子文件夹，并且您想要与组 A 和 B 共享一个子文件夹，并且只允许组访问第二个子文件夹，请与组 A 共享父文件夹，并将组 B 添加到第一个子文件夹中。</span><span class="sxs-lookup"><span data-stu-id="27598-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="27598-111">停止共享文件或文件夹</span><span class="sxs-lookup"><span data-stu-id="27598-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

