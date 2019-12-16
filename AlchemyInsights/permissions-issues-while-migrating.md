---
title: 迁移时的权限问题
ms.author: pebaum
author: pebaum
ms.date: 9/18/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 95bfbfdf002e457230479a860058c1cf7ab1f8c2
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054404"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="3c5d8-102">用户配置文件和照片同步</span><span class="sxs-lookup"><span data-stu-id="3c5d8-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="3c5d8-103">**个人资料照片同步**-用户可能会注意到，他们的个人资料照片未与 SharePoint 同步。</span><span class="sxs-lookup"><span data-stu-id="3c5d8-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="3c5d8-104">或者，他们可能尝试更新其个人资料照片，并且该照片仍显示为旧照片。</span><span class="sxs-lookup"><span data-stu-id="3c5d8-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="3c5d8-105">若要确保个人资料照片按预期方式显示，用户需要启动照片同步。</span><span class="sxs-lookup"><span data-stu-id="3c5d8-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="3c5d8-106">有关照片同步过程的详细信息，请参阅[有关 Office 365 中的配置文件图片同步的信息](https://go.microsoft.com/fwlink/?linkid=2022634)</span><span class="sxs-lookup"><span data-stu-id="3c5d8-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Office 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="3c5d8-107">**配置文件同步**-完成配置文件同步所需的时间取决于 AD 导入作业必须处理的更改（工时）数。</span><span class="sxs-lookup"><span data-stu-id="3c5d8-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="3c5d8-108">如果有很多更改，计时器作业将执行大量工作，并且将需要更长时间才能在用户配置文件应用程序中反映这些更改。</span><span class="sxs-lookup"><span data-stu-id="3c5d8-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="3c5d8-109">如果计时器作业的工时量较少，则更改将在用户配置文件应用程序中反应得更快。</span><span class="sxs-lookup"><span data-stu-id="3c5d8-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="3c5d8-110">有关配置文件同步过程的详细信息，请参阅[SharePoint Online 中有关用户配置文件同步的信息](https://go.microsoft.com/fwlink/?linkid=2022639)</span><span class="sxs-lookup"><span data-stu-id="3c5d8-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="3c5d8-111">**更新 Office delve 中的配置文件**-delve 用户可以管理其 Office 365 配置文件。</span><span class="sxs-lookup"><span data-stu-id="3c5d8-111">**Update Profile in Office Delve** - Delve users can manage their Office 365 Profile.</span></span> <span data-ttu-id="3c5d8-112">有关详细信息，请参阅[在 Office Delve 中查看和更新您的配置文件](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)。</span><span class="sxs-lookup"><span data-stu-id="3c5d8-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

