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
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer 连接问题 

如果 SharePoint Designer 在 SharePoint 网站中遇到连接问题, 请尝试以下常见解决方案。

步骤 1: 验证 SharePoint Designer 是否已更新。

- [SharePoint Designer 2013](https://www.microsoft.com/download/details.aspx?id=35491)

- [SharePoint Designer Service Pack 1 (SP1)](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)

- [SharePoint Designer 2013 更新 (KB3114721)](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)

步骤 2: 清除本地缓存文件

- 关闭 SharePoint Designer 2013。

- 在本地计算机上, 浏览到以下文件夹以删除缓存的文件。

- 单击 "启动", 运行并删除在以下每个位置下找到的所有文件。

%APPDATA%\Microsoft\Web Server Extensions\Cache%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

打开 SharePoint Designer 2013, 然后再次输入帐户以查看它是否正常工作。

步骤 3:[为 Windows 设备上的 Office 2013 启用新式验证](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)

步骤 4: 管理员将需要允许自定义脚本允许 SharePoint Designer 连接。

有关详细步骤、示例和注意事项, 请参阅[Allow or 预防自定义脚本](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)。


