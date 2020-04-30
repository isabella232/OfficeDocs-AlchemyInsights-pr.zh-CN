---
title: MC210173 - SharePoint Designer 新自定义窗体功能弃用
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 185e8fc94345b240667490b1ffc63af8459d8daf
ms.sourcegitcommit: a9e6b2fcce8bd12fd079ed967f426b67d5c6d239
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43928518"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="78a98-102">MC210173 - SharePoint Designer 新自定义窗体功能弃用</span><span class="sxs-lookup"><span data-stu-id="78a98-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="78a98-103">我们发现了一个会影响 SharePoint Online 中[创建自定义窗体](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2)的 SharePoint Designer 功能的问题。</span><span class="sxs-lookup"><span data-stu-id="78a98-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="78a98-104">仔细检查后，我们确定尚无此问题的解决方法，并已选择禁用自定义窗体创建功能，自 2020 年 4 月 25 日星期六 UTC 凌晨 3:00 起生效。</span><span class="sxs-lookup"><span data-stu-id="78a98-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="78a98-105">此更改不会影响在 SharePoint Online Designer 中编辑以前创建的窗体的能力或其他现有功能。</span><span class="sxs-lookup"><span data-stu-id="78a98-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="78a98-106">进行此更改后，用户在创建新窗体时可能收到错误：“无法将列表更改保存到服务器”。</span><span class="sxs-lookup"><span data-stu-id="78a98-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="78a98-107">以前曾利用 SharePoint Designer 创建自定义窗体的用户可以使用 [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) 来实现此目的。</span><span class="sxs-lookup"><span data-stu-id="78a98-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="78a98-108">PowerApps 是一款简单而强大的工具，它使用户可以在 SharePoint Online Modern 体验中操作，直接从浏览器窗口创建和编辑 SharePoint 列表和文档库的自定义窗体。</span><span class="sxs-lookup"><span data-stu-id="78a98-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="78a98-109">PowerApps 不需要传统编码知识或下载任何其他应用（如 InfoPath）。</span><span class="sxs-lookup"><span data-stu-id="78a98-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="78a98-110">**注意**：SharePoint Online Classic 用户需要暂时切换到 Modern 体验以便访问和使用 PowerApps；但是，SharePoint Online Classic 体验用户可以访问在 PowerApps 中创建的所有自定义窗体。</span><span class="sxs-lookup"><span data-stu-id="78a98-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
