---
title: SharePoint Designer 连接问题
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: a4aeaeaea5743c276b907c78317ff30f5610be81
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36508413"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="663ef-102">SharePoint Designer 连接问题</span><span class="sxs-lookup"><span data-stu-id="663ef-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="663ef-103">如果 SharePoint Designer 遇到 SharePoint 网站的连接问题, 请尝试以下常见解决方案。</span><span class="sxs-lookup"><span data-stu-id="663ef-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="663ef-104">步骤 1: 验证 sharepoint designer 2013 是否已更新 sharepoint designer [Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)和[8 月2日, 2016 Update for sharepoint designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)。</span><span class="sxs-lookup"><span data-stu-id="663ef-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="663ef-105">步骤 2: 清除本地缓存文件:</span><span class="sxs-lookup"><span data-stu-id="663ef-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="663ef-106">关闭 SharePoint Designer 2013。</span><span class="sxs-lookup"><span data-stu-id="663ef-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="663ef-107">在本地计算机上, 删除在以下每个文件夹中找到的所有文件。</span><span class="sxs-lookup"><span data-stu-id="663ef-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="663ef-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="663ef-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="663ef-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="663ef-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="663ef-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="663ef-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="663ef-111">打开 SharePoint Designer 2013, 然后再次输入帐户以查看它是否正常工作。</span><span class="sxs-lookup"><span data-stu-id="663ef-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="663ef-112">步骤 3:[为 Windows 设备上的 Office 2013 启用新式验证](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="663ef-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="663ef-113">步骤 4: 管理员将需要允许 sharepoint 管理中心设置中的**自定义脚本**, 以允许 sharepoint Designer 连接。</span><span class="sxs-lookup"><span data-stu-id="663ef-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="663ef-114">有关详细信息, 请参阅[允许或阻止自定义脚本](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)。</span><span class="sxs-lookup"><span data-stu-id="663ef-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


