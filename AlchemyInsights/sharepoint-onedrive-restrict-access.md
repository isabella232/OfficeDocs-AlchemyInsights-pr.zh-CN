---
title: 在 SharePoint 或 OneDrive 中限制访问权限
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 5101366ff65f477c19b9c7f2c0d7065cf88501b0
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2019
ms.locfileid: "34735133"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="7754c-102">在 SharePoint 或 OneDrive 中限制访问权限</span><span class="sxs-lookup"><span data-stu-id="7754c-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="7754c-103">有多种方法可以限制对 SharePoint Online/OneDrive 服务的访问。</span><span class="sxs-lookup"><span data-stu-id="7754c-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="7754c-104">下面概述了这些不同的访问限制方法。</span><span class="sxs-lookup"><span data-stu-id="7754c-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="7754c-105">权限限制</span><span class="sxs-lookup"><span data-stu-id="7754c-105">Permission Restriction</span></span>

<span data-ttu-id="7754c-106">在 SharePoint Online 和 OneDrive for business 中, 我们仅授予对应具有访问权限的那些组/个人的访问权限, 从而限制对网站、文件和文件夹等项目的访问。</span><span class="sxs-lookup"><span data-stu-id="7754c-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

[<span data-ttu-id="7754c-107">自定义 SharePoint 列表或库的权限</span><span class="sxs-lookup"><span data-stu-id="7754c-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/en-us/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[<span data-ttu-id="7754c-108">自定义 SharePoint 网站权限</span><span class="sxs-lookup"><span data-stu-id="7754c-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions)

[<span data-ttu-id="7754c-109">更改针对子文件夹的权限</span><span class="sxs-lookup"><span data-stu-id="7754c-109">Change the permissions on a subfolder</span></span>](https://support.office.com/en-us/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[<span data-ttu-id="7754c-110">通过非托管设备控制访问</span><span class="sxs-lookup"><span data-stu-id="7754c-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/en-us/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="7754c-111">作为 Office 365 中的 SharePoint 或全局管理员, 您可以阻止或限制对来自非托管设备 (在 Intune 中未加入或合规性的混合式 AD) 的 SharePoint 和 OneDrive 内容的访问权限。</span><span class="sxs-lookup"><span data-stu-id="7754c-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="7754c-112">网络位置限制</span><span class="sxs-lookup"><span data-stu-id="7754c-112">Network Location Restriction</span></span>

<span data-ttu-id="7754c-113">作为 IT 管理员, 您可以根据您信任的已定义网络位置来控制对 SharePoint 和 OneDrive 资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="7754c-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="7754c-114">这也称为基于位置的策略。</span><span class="sxs-lookup"><span data-stu-id="7754c-114">This is also known as location-based policy.</span></span> <span data-ttu-id="7754c-115">有关详细信息, 请参阅[基于网络位置控制对 SharePoint Online 和 OneDrive 数据的访问](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="7754c-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/en-us/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="7754c-116">网站锁定限制</span><span class="sxs-lookup"><span data-stu-id="7754c-116">Site Lock Restriction</span></span> 

<span data-ttu-id="7754c-117">在 SharePoint Online 中, 您可以锁定网站集, 因此没有人能够访问。</span><span class="sxs-lookup"><span data-stu-id="7754c-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="7754c-118">这是通过使用[get-sposite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState 属性的 PowerShell 和[SharePoint Online 命令行管理](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)程序设置的。</span><span class="sxs-lookup"><span data-stu-id="7754c-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="7754c-119">限制用户创建网站或子网站</span><span class="sxs-lookup"><span data-stu-id="7754c-119">Restrict users from creating sites or subsites</span></span>

<span data-ttu-id="7754c-120">作为 SharePoint 管理员或 Office 365 全局管理员, 你可以让你的用户创建和管理自己的 SharePoint 网站, 确定可以创建的网站类型, 并指定网站的位置。</span><span class="sxs-lookup"><span data-stu-id="7754c-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="7754c-121">有关详细信息, 请参阅[在 SharePoint Online 中管理网站创建](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="7754c-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/en-us/sharepoint/manage-site-creation)</span></span>

