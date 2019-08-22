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
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer 连接问题 

如果 SharePoint Designer 遇到 SharePoint 网站的连接问题, 请尝试以下常见解决方案。

步骤 1: 验证 sharepoint designer 2013 是否已更新 sharepoint designer [Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)和[8 月2日, 2016 Update for sharepoint designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)。



步骤 2: 清除本地缓存文件:

1. 关闭 SharePoint Designer 2013。

2. 在本地计算机上, 删除在以下每个文件夹中找到的所有文件。

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. 打开 SharePoint Designer 2013, 然后再次输入帐户以查看它是否正常工作。

步骤 3:[为 Windows 设备上的 Office 2013 启用新式验证](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide)。

步骤 4: 管理员将需要允许 sharepoint 管理中心设置中的**自定义脚本**, 以允许 sharepoint Designer 连接。 有关详细信息, 请参阅[允许或阻止自定义脚本](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)。


