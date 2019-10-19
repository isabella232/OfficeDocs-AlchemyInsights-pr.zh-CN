---
title: 在 SharePoint 或 OneDrive 中限制访问权限
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750654"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>在 SharePoint 或 OneDrive 中限制访问权限

有多种方法可以限制对 SharePoint Online/OneDrive 服务的访问。 下面概述了这些不同的访问限制方法。 

**权限限制**

在 SharePoint Online 和 OneDrive for business 中，我们仅授予对应具有访问权限的那些组/个人的访问权限，从而限制对网站、文件和文件夹等项目的访问。

- [自定义 SharePoint 列表或库的权限](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [自定义 SharePoint 网站权限](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [更改针对子文件夹的权限](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [通过非托管设备控制访问](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

作为 Office 365 中的 SharePoint 或全局管理员，您可以阻止或限制对来自非托管设备（在 Intune 中未加入或合规性的混合式 AD）的 SharePoint 和 OneDrive 内容的访问权限。

**网络位置限制**

作为 IT 管理员，您可以根据您信任的已定义网络位置来控制对 SharePoint 和 OneDrive 资源的访问权限。 这也称为基于位置的策略。 有关详细信息，请参阅[基于网络位置控制对 SharePoint Online 和 OneDrive 数据的访问](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**网站锁定限制** 

在 SharePoint Online 中，您可以锁定网站集，因此没有人能够访问。 这是通过使用[get-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState 属性的 PowerShell 和[SharePoint Online 命令行管理](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)程序设置的。

**限制用户创建网站或子网站**

作为 SharePoint 管理员或 Office 365 全局管理员，你可以让你的用户创建和管理自己的 SharePoint 网站，确定可以创建的网站类型，并指定网站的位置。 有关详细信息，请参阅[在 SharePoint Online 中管理网站创建](https://docs.microsoft.com/sharepoint/manage-site-creation)

