---
title: 配置文件同步
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554323"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="6d333-102">何时将我的配置文件更改同步到 SharePoint 用户配置文件应用程序？</span><span class="sxs-lookup"><span data-stu-id="6d333-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="6d333-103">SharePoint Online 使用 Active Directory 导入计时器作业（AD 导入）将用户和组导入到用户配置文件应用程序中。</span><span class="sxs-lookup"><span data-stu-id="6d333-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="6d333-104">AD 导入将更改从 SharePoint Online 目录存储同步到用户配置文件应用程序。</span><span class="sxs-lookup"><span data-stu-id="6d333-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="6d333-105">这些更改在批处理中进行处理。</span><span class="sxs-lookup"><span data-stu-id="6d333-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="6d333-106">计时器作业将一直运行，直到更改被同步。</span><span class="sxs-lookup"><span data-stu-id="6d333-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="6d333-107">作业运行所需的时间取决于要处理的更改数量。</span><span class="sxs-lookup"><span data-stu-id="6d333-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="6d333-108">大量更改需要较长时间。</span><span class="sxs-lookup"><span data-stu-id="6d333-108">A large number of changes takes longer.</span></span> <span data-ttu-id="6d333-109">服务级别协议（SLA）指出对 SharePoint Online 目录中的用户所做的更改将在24小时内反映到用户配置文件应用程序中。</span><span class="sxs-lookup"><span data-stu-id="6d333-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="6d333-110">有关 SharePoint Online 中的用户配置文件同步的详细信息</span><span class="sxs-lookup"><span data-stu-id="6d333-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

