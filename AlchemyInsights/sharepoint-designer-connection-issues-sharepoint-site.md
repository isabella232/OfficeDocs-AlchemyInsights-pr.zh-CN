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
ms.openlocfilehash: 7451cfe957545537298f57feb5b47bd6d43cddbf
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716882"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Designer 连接问题 

<p>如果 SharePoint Designer 在 SharePoint 网站中遇到连接问题, 请尝试以下常见解决方案。</p> <p><strong>步骤 1:</strong><strong>验证 SharePoint Designer 是否已&nbsp;更新</strong></p> <ul> <li><a href="https://www.microsoft.com/en-us/download/details.aspx?id=35491">SharePoint Designer 2013</a></li> <li><a href="https://support.microsoft.com/en-us/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1">SharePoint Designer Service Pack 1 (SP1)</a></li> <li><a href="https://support.microsoft.com/en-us/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721">SharePoint Designer 2013 更新 (KB3114721)</a></li> </ul> <p><strong>步骤 2:</strong><strong>清除本地缓存文件</strong>&nbsp;</p> <ol> <li style="font-weight: 400;">关闭 SharePoint Designer 2013。&nbsp;</li> <li style="font-weight: 400;">在本地计算机上, 浏览到以下文件夹以删除缓存的文件。&nbsp;</li> <li style="font-weight: 400;">单击 "<strong>开始&gt; "-"运行</strong>", 然后删除在以下每个位置下找到的所有文件。&nbsp;<br /><br />%APPDATA%\Microsoft\Web Server Extensions\Cache<br />%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache<br />%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</li> <li style="font-weight: 400;">打开 SharePoint Designer 2013, 然后再次输入帐户以查看它是否正常工作。</li> </ol> <p><strong>步骤 3:</strong><a href="https://docs.microsoft.com/en-us/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=%252fen-us%252farticle%252fEnable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&amp;view=o365-worldwide"><strong>在 Windows 设备上为 Office 2013 启用新式验证</strong></a>&nbsp;</p> <p><strong>步骤 4:</strong><strong>管理员将需要允许自定义脚本允许 SharePoint Designer 连接</strong>。</p> <p>有关详细步骤、示例和注意事项, 请参阅<a href="https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script">Allow or 预防自定义脚本</a>。&nbsp;</p>


