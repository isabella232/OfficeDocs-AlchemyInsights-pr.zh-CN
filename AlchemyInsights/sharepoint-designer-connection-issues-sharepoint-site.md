---
title: SharePoint Designer 连接问题
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 01ccc6bc28148f397fb6cd2b7a0eaaeb5b51973f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511534"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="7a307-102">SharePoint Designer 连接问题</span><span class="sxs-lookup"><span data-stu-id="7a307-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="7a307-103">如果 SharePoint Designer 遇到 SharePoint 网站的连接问题，请尝试以下常见解决方案。</span><span class="sxs-lookup"><span data-stu-id="7a307-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="7a307-104">步骤1：验证 sharepoint designer 2013 是否已更新 sharepoint designer [Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)和[8 月2日，2016 Update for sharepoint designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)。</span><span class="sxs-lookup"><span data-stu-id="7a307-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="7a307-105">步骤2：清除本地缓存文件：</span><span class="sxs-lookup"><span data-stu-id="7a307-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="7a307-106">关闭 SharePoint Designer 2013。</span><span class="sxs-lookup"><span data-stu-id="7a307-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="7a307-107">在本地计算机上，删除在以下每个文件夹中找到的所有文件。</span><span class="sxs-lookup"><span data-stu-id="7a307-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="7a307-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span><span class="sxs-lookup"><span data-stu-id="7a307-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="7a307-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="7a307-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="7a307-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="7a307-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="7a307-111">打开 SharePoint Designer 2013，然后再次输入帐户以查看它是否正常工作。</span><span class="sxs-lookup"><span data-stu-id="7a307-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="7a307-112">步骤3：[为 Windows 设备上的 Office 2013 启用新式验证](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)。</span><span class="sxs-lookup"><span data-stu-id="7a307-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>

<span data-ttu-id="7a307-113">步骤4：管理员将需要允许 sharepoint 管理中心设置中的**自定义脚本**，以允许 sharepoint Designer 连接。</span><span class="sxs-lookup"><span data-stu-id="7a307-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="7a307-114">有关详细信息，请参阅[允许或阻止自定义脚本](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)。</span><span class="sxs-lookup"><span data-stu-id="7a307-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


