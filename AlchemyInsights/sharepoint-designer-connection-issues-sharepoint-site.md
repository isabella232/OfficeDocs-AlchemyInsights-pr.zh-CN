---
title: SharePoint Online 权限级别
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 356fef8e02f2c1fd9d209c68194685bb0acaa367
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760683"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="f6900-102">SharePoint Designer 连接问题</span><span class="sxs-lookup"><span data-stu-id="f6900-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="f6900-103">如果 SharePoint Designer 在 SharePoint 网站中遇到连接问题, 请尝试以下常见解决方案。</span><span class="sxs-lookup"><span data-stu-id="f6900-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please attempt the following common solutions.</span></span>

<span data-ttu-id="f6900-104">步骤 1: 验证 SharePoint Designer 是否已更新。</span><span class="sxs-lookup"><span data-stu-id="f6900-104">Step 1: Verify SharePoint Designer is updated.</span></span>

- [<span data-ttu-id="f6900-105">SharePoint Designer 2013</span><span class="sxs-lookup"><span data-stu-id="f6900-105">SharePoint Designer 2013</span></span>](https://www.microsoft.com/download/details.aspx?id=35491)

- [<span data-ttu-id="f6900-106">SharePoint Designer Service Pack 1 (SP1)</span><span class="sxs-lookup"><span data-stu-id="f6900-106">SharePoint Designer Service Pack 1 (SP1)</span></span>](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [<span data-ttu-id="f6900-107">SharePoint Designer 2013 更新 (KB3114721)</span><span class="sxs-lookup"><span data-stu-id="f6900-107">Update for SharePoint Designer 2013 (KB3114721)</span></span>](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

<span data-ttu-id="f6900-108">步骤 2: 清除本地缓存文件</span><span class="sxs-lookup"><span data-stu-id="f6900-108">Step 2: Clear the local cache files</span></span>

- <span data-ttu-id="f6900-109">关闭 SharePoint Designer 2013。</span><span class="sxs-lookup"><span data-stu-id="f6900-109">Close SharePoint Designer 2013.</span></span>

- <span data-ttu-id="f6900-110">在本地计算机上, 浏览到以下文件夹以删除缓存的文件。</span><span class="sxs-lookup"><span data-stu-id="f6900-110">On the local computer, browse to the following folders to remove cached files.</span></span>

- <span data-ttu-id="f6900-111">单击 "启动", 运行并删除在以下每个位置下找到的所有文件。</span><span class="sxs-lookup"><span data-stu-id="f6900-111">Click Start, Run and delete all files found under each of the below locations.</span></span>

<span data-ttu-id="f6900-112">%APPDATA%\Microsoft\Web Server Extensions\Cache%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="f6900-112">%APPDATA%\Microsoft\Web Server Extensions\Cache %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

<span data-ttu-id="f6900-113">打开 SharePoint Designer 2013, 然后再次输入帐户以查看它是否正常工作。</span><span class="sxs-lookup"><span data-stu-id="f6900-113">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="f6900-114">步骤 3:[为 Windows 设备上的 Office 2013 启用新式验证](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="f6900-114">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)</span></span>

<span data-ttu-id="f6900-115">步骤 4: 管理员将需要允许自定义脚本允许 SharePoint Designer 连接。</span><span class="sxs-lookup"><span data-stu-id="f6900-115">Step 4: Administrators will need to Allow Custom Script to allow the SharePoint Designer connection.</span></span>

<span data-ttu-id="f6900-116">有关详细步骤、示例和注意事项, 请参阅[Allow or 预防自定义脚本](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)。</span><span class="sxs-lookup"><span data-stu-id="f6900-116">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


