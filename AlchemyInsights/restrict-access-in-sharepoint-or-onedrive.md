---
title: 限制在 SharePoint 或 OneDrive 中的访问
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29459343"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="2df78-102">限制在 SharePoint 或 OneDrive 中的访问</span><span class="sxs-lookup"><span data-stu-id="2df78-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="2df78-p101">在 SharePoint 和 OneDrive 中，您限制对像文件、 文件夹和列表项的访问仅对组或个人所需具有访问权限授予的访问权限。默认情况下，在 SharePoint 中的权限继承从较高层次结构中。因此，文件从其权限继承的库，从网站中继承其权限的文件夹继承其权限。</span><span class="sxs-lookup"><span data-stu-id="2df78-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="2df78-p102">您可以共享在高级别 (例如通过共享整个网站) 然后中断继承，如果您不希望共享网站上的所有项目。但是，我们建议不要这因为它使保留的权限，以便将来更复杂的和混乱。下面是您所能做的改为：</span><span class="sxs-lookup"><span data-stu-id="2df78-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="2df78-109">如果，例如，要共享的文件夹中的一个文件除外的所有内容，请将该文件移动到一个不共享的新位置。</span><span class="sxs-lookup"><span data-stu-id="2df78-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="2df78-110">如果您有两个的子文件夹中，并且想要组 A 和 B 与共享一个子文件夹和只允许组 A 访问到第二个子文件夹、 与组的共享的父文件夹和将组 B 添加到第一个子文件夹。</span><span class="sxs-lookup"><span data-stu-id="2df78-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="2df78-111">停止共享文件或文件夹</span><span class="sxs-lookup"><span data-stu-id="2df78-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

