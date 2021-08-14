---
title: SharePoint设计器连接问题
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942015"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint设计器连接问题 

如果SharePoint设计器遇到与网站SharePoint问题，请尝试以下常见解决方案。

步骤 1：验证 SharePoint Designer 2013 已使用[SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1)和 SharePoint Designer [2013 的 2016](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)年 8 月 2 日更新进行了更新。



步骤 2：清除本地缓存文件：

1. 关闭SharePoint Designer 2013。

2. 在本地计算机上，删除以下每个文件夹中找到的所有文件。

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. 打开 SharePoint Designer 2013，然后再次输入帐户以查看其是否正常工作。

步骤 3：在 Windows 设备上为[Office 2013 启用新式验证](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)。

步骤 4：管理员将需要在管理中心设置中SharePoint自定义脚本，以允许SharePoint设计器连接。 有关详细信息 [，请参阅允许或阻止](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) 自定义脚本。


