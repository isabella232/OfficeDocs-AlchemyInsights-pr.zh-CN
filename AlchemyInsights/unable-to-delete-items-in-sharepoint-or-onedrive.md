---
title: 无法删除 SharePoint 或 OneDrive 中的项目
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511966"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="fcc34-102">无法删除项目</span><span class="sxs-lookup"><span data-stu-id="fcc34-102">Unable to delete items</span></span>

<span data-ttu-id="fcc34-103">保留策略可以导致这种情况，您需要禁用或排除导致此问题的相应保留。</span><span class="sxs-lookup"><span data-stu-id="fcc34-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="fcc34-104">在删除保留策略或保留后，可能需要长达24小时才能使更改生效。</span><span class="sxs-lookup"><span data-stu-id="fcc34-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="fcc34-105">确保项目上没有[保留策略](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)设置。</span><span class="sxs-lookup"><span data-stu-id="fcc34-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="fcc34-106">网站可能已超出存储限制，请增加[网站配额](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)并删除该项。</span><span class="sxs-lookup"><span data-stu-id="fcc34-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="fcc34-107">确保该项目未[签出](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)给其他用户。</span><span class="sxs-lookup"><span data-stu-id="fcc34-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="fcc34-108">最后，管理员可以使用[SharePoint 模式和做法](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation)（PnP），其中包含一个 PowerShell 命令库，这些命令允许您执行复杂的管理操作，例如强制删除 stubborn 项目。</span><span class="sxs-lookup"><span data-stu-id="fcc34-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="fcc34-109">删除 PNP 文件</span><span class="sxs-lookup"><span data-stu-id="fcc34-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="fcc34-110">删除 PNP 文件夹</span><span class="sxs-lookup"><span data-stu-id="fcc34-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="fcc34-111">删除 PNP 列表项</span><span class="sxs-lookup"><span data-stu-id="fcc34-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="fcc34-112">删除 PNP 列表</span><span class="sxs-lookup"><span data-stu-id="fcc34-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="fcc34-113">删除 PNP 字段（列）</span><span class="sxs-lookup"><span data-stu-id="fcc34-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)