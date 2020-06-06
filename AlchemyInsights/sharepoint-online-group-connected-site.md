---
title: 将组添加到 SharePoint 网站
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582801"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>在 SharePoint 中创建组连接网站时出现的问题

1. 创建或重新创建组连接的网站时遇到的一些常见问题。
如果已删除某个组及其连接的网站，并且想要创建另一个具有相同 URL 的网站，则需要永久删除以前的网站。

   - 下载[SPO 命令行管理](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)程序
   - 有关如何开始使用 Powershell 的详细信息，请参阅[SharePoint Online 命令行管理](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)程序入门。
   - 使用[Remove-spodeletedsite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell Cmdlet 从已删除网站中删除网站。 需要 Powershell 以永久删除组网站。

1. 如果您正在创建一个组连接的网站并收到警告：**另一个具有相同别名的组已存在**，请从[Microsoft 365 管理中心](https://admin.microsoft.com/AdminPortal/Home#/groups)检查现有组。 若要解决此问题，请删除现有组（如果不再需要它）或创建具有分配了不同别名的网站。

1. 可以使用不同的方法来创建和使用 SharePoint 的新式组。

   - 您可以将现有网站连接到 Microsoft 365 组。 有关详细信息，请参阅[使用 SharePoint 用户界面连接 Microsoft 365 组](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)。
   - 若要创建 Microsoft 365 组连接的网站，您需要创建一个[团队网站](https://admin.microsoft.com/sharepoint)。
