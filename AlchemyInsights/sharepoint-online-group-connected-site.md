---
title: 将组添加到 SharePoint 网站
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582801"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="bafcd-102">在 SharePoint 中创建组连接网站时出现的问题</span><span class="sxs-lookup"><span data-stu-id="bafcd-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="bafcd-103">创建或重新创建组连接的网站时遇到的一些常见问题。</span><span class="sxs-lookup"><span data-stu-id="bafcd-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="bafcd-104">如果已删除某个组及其连接的网站，并且想要创建另一个具有相同 URL 的网站，则需要永久删除以前的网站。</span><span class="sxs-lookup"><span data-stu-id="bafcd-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="bafcd-105">下载[SPO 命令行管理](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)程序</span><span class="sxs-lookup"><span data-stu-id="bafcd-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="bafcd-106">有关如何开始使用 Powershell 的详细信息，请参阅[SharePoint Online 命令行管理](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)程序入门。</span><span class="sxs-lookup"><span data-stu-id="bafcd-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="bafcd-107">使用[Remove-spodeletedsite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell Cmdlet 从已删除网站中删除网站。</span><span class="sxs-lookup"><span data-stu-id="bafcd-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="bafcd-108">需要 Powershell 以永久删除组网站。</span><span class="sxs-lookup"><span data-stu-id="bafcd-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="bafcd-109">如果您正在创建一个组连接的网站并收到警告：**另一个具有相同别名的组已存在**，请从[Microsoft 365 管理中心](https://admin.microsoft.com/AdminPortal/Home#/groups)检查现有组。</span><span class="sxs-lookup"><span data-stu-id="bafcd-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="bafcd-110">若要解决此问题，请删除现有组（如果不再需要它）或创建具有分配了不同别名的网站。</span><span class="sxs-lookup"><span data-stu-id="bafcd-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="bafcd-111">可以使用不同的方法来创建和使用 SharePoint 的新式组。</span><span class="sxs-lookup"><span data-stu-id="bafcd-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="bafcd-112">您可以将现有网站连接到 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="bafcd-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="bafcd-113">有关详细信息，请参阅[使用 SharePoint 用户界面连接 Microsoft 365 组](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)。</span><span class="sxs-lookup"><span data-stu-id="bafcd-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="bafcd-114">若要创建 Microsoft 365 组连接的网站，您需要创建一个[团队网站](https://admin.microsoft.com/sharepoint)。</span><span class="sxs-lookup"><span data-stu-id="bafcd-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
