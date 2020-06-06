---
title: 权限继承
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bb5c440a-ca70-4dc6-b517-688e80551101
ms.openlocfilehash: 791085593433dcad9b800fdea8c7ea4a878604e7
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581041"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="219e0-102">权限继承在 SharePoint 中的工作方式</span><span class="sxs-lookup"><span data-stu-id="219e0-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="219e0-103">默认情况下，SharePoint 中的权限从层次结构中的较高版本继承。</span><span class="sxs-lookup"><span data-stu-id="219e0-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="219e0-104">因此，文件从文件夹继承其权限，这将从库继承其权限，这会从网站继承其权限，这将从网站集继承权限。</span><span class="sxs-lookup"><span data-stu-id="219e0-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="219e0-105">有关删除唯一权限和还原继承的信息，请参阅[编辑和管理列表或库的权限](https://go.microsoft.com/fwlink/?linkid=869946)。</span><span class="sxs-lookup"><span data-stu-id="219e0-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

