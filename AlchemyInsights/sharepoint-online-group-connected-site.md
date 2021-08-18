---
title: 将组添加到SharePoint网站
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8166c2a19e5849de6caace4eea0fee5866f5adc3bfc2c483f18fc788c1bf2fa9
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57897706"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>在网站中创建组连接的站点时SharePoint

1. 如果已删除组及其连接的站点，并且希望创建另一个 URL 相同的网站，则需要永久删除以前的网站。

   - 下载 [SPO 命令行管理程序](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - 有关 Powershell 入门详细信息，请参阅 SharePoint [Online 命令行管理程序 入门](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)。
   - 使用 [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet 从已删除的站点中删除站点。 需要 Powershell 才能永久删除组网站。

1. 如果要创建已连接组的网站并收到一条警告：已存在另一个同名的组，请检查现有组[Microsoft 365 管理中心。](https://admin.microsoft.com/AdminPortal/Home#/groups) 若要解决此问题，请删除现有组（如果不再需要）或创建分配了不同别名的网站。

1. 有不同方法可以创建新式组并使用新式SharePoint。

   - 可以将现有网站连接到Microsoft 365组。 有关详细信息，请参阅[连接用户界面Microsoft 365组SharePoint组](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)。
   - 若要创建Microsoft 365组连接的站点，需要创建团队[网站](https://admin.microsoft.com/sharepoint)。
