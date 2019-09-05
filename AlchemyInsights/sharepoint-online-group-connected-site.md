---
title: 将组添加到 SharePoint 网站
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 423db4e5bbb85e75aee3548d5b6b46a64ebc6fa0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750510"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="d213a-102">在 SharePoint Online 中创建或组合连接的网站时出现的问题</span><span class="sxs-lookup"><span data-stu-id="d213a-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="d213a-103">创建或重新创建组连接的网站时遇到了几个常见的问题。</span><span class="sxs-lookup"><span data-stu-id="d213a-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="d213a-104">如果已删除某个组及其连接的网站，并且想要创建另一个具有相同 URL 的网站，则需要永久删除以前的网站。</span><span class="sxs-lookup"><span data-stu-id="d213a-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="d213a-105">下载[SPO 命令行管理](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)程序</span><span class="sxs-lookup"><span data-stu-id="d213a-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="d213a-106">有关如何开始使用 powershell 的详细信息，请参阅[SharePoint Online 命令行管理](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)程序入门</span><span class="sxs-lookup"><span data-stu-id="d213a-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="d213a-107">使用[remove-spodeletedsite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell Cmdlet 从已删除网站中删除网站。</span><span class="sxs-lookup"><span data-stu-id="d213a-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="d213a-108">如果您正在创建一个组连接的网站并收到一条警告，并且已存在另一个具有相同别名的组，请[从管理中心检查 Office 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups)中的现有组。</span><span class="sxs-lookup"><span data-stu-id="d213a-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="d213a-109">若要解决此问题，请删除现有组（如果不再需要它）或创建具有分配了不同别名的网站。</span><span class="sxs-lookup"><span data-stu-id="d213a-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="d213a-110">可以使用不同的方法来创建和使用 SharePoint 的新式组。</span><span class="sxs-lookup"><span data-stu-id="d213a-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="d213a-111">您可以将现有网站连接到 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="d213a-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="d213a-112">有关详细信息，请参阅[Connect a Office 365 group using The SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)。</span><span class="sxs-lookup"><span data-stu-id="d213a-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="d213a-113">若要创建 Office 365 组连接的网站，需要创建团队网站。</span><span class="sxs-lookup"><span data-stu-id="d213a-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="d213a-114">有关详细信息，请参阅[在 SharePoint 中创建团队网站](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)。</span><span class="sxs-lookup"><span data-stu-id="d213a-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

