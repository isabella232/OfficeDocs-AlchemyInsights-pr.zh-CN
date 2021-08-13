---
title: 限制访问SharePoint或OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093799"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>限制访问SharePoint或OneDrive

有许多方法可以限制对 SharePoint Online/OneDrive的访问。 下面概述了这些各种访问限制方法。 

**权限限制**

在 SharePoint Online 和 OneDrive for Business 中，我们仅向应具有访问权限的组/个人授予访问权限，从而限制对网站、文件和文件夹等项目的访问权限。

- [自定义列表或库SharePoint权限](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [自定义 SharePoint 网站权限](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [更改针对子文件夹的权限](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [控制来自非托管设备的访问](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

作为SharePoint管理员或全局管理员，你可以阻止或限制非托管设备（未加入混合 AD 或在 Intune) 中未加入混合 AD (）访问 SharePoint 和 OneDrive 内容。

**网络位置限制**

作为 IT 管理员，你可以根据你信任SharePoint OneDrive定义网络位置来控制对资源的访问权限。 这也称为基于位置的策略。 有关详细信息，请参阅控制对[SharePoint Online 的访问和OneDrive基于网络位置的数据](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**网站锁定限制** 

在 SharePoint Online 中，您可以锁定网站集，因此没有人可以访问。 这是通过 PowerShell 和[SharePoint Online 命令行](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)管理程序使用[Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState 属性设置的。

**限制用户创建网站或子网站**

作为SharePoint管理员或全局管理员，你可以让用户创建和管理自己的 SharePoint 网站，确定他们可以创建的网站类型，并指定网站的位置。 有关详细信息，请参阅在[SharePoint Online 中管理网站创建](https://docs.microsoft.com/sharepoint/manage-site-creation)

