---
title: 配置文件同步
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a32cf9e623d1be7a2c85ef4951c6eb7f001b7db0
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28277427"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="a37da-102">何时我的配置文件更改同步到 SharePoint 用户配置文件应用程序？</span><span class="sxs-lookup"><span data-stu-id="a37da-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="a37da-103">SharePoint Online 使用 Active Directory 导入计时器作业 （AD 导入） 导入用户配置文件应用程序的用户和组。</span><span class="sxs-lookup"><span data-stu-id="a37da-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="a37da-p101">AD 导入同步从 SharePoint Online 目录存储更改为用户配置文件应用程序。批量处理的这些更改。</span><span class="sxs-lookup"><span data-stu-id="a37da-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="a37da-106">计时器作业运行，直到同步所做的更改。</span><span class="sxs-lookup"><span data-stu-id="a37da-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="a37da-p102">要运行的作业的时间取决于要处理的更改的数量。大量更改的时间。服务级别协议 (SLA) 指明，将在 24 小时内中用户配置文件应用程序中反映到 SharePoint Online 目录中的用户的更改。</span><span class="sxs-lookup"><span data-stu-id="a37da-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="a37da-110">有关 SharePoint Online 中的用户配置文件同步的详细信息</span><span class="sxs-lookup"><span data-stu-id="a37da-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

