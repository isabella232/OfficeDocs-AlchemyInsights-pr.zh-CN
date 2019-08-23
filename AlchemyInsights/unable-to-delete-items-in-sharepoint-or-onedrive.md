---
title: 无法删除 SharePoint 或 OneDrive 中的项目
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: b25e6d144dcefcfed4258e78ad5cfd4089ba7d1e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558643"
---
# <a name="unable-to-delete-items"></a>无法删除项目

删除 SharePoint 项时遇到问题？

- 请始终确保你具有删除项目的[相应权限](https://docs.microsoft.com/sharepoint/default-sharepoint-groups), 或让[网站集管理员](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator)尝试删除该项目。

- 确保项目上没有[保留策略](https://docs.microsoft.com/office365/securitycompliance/retention-policies)设置。

- 确保该项目未[签出](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)给其他用户。

- 最后, 管理员可以使用[SharePoint 模式和做法](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation)(PnP), 其中包含一个 PowerShell 命令库, 这些命令允许您执行复杂的管理操作, 例如强制删除 stubborn 项目。
- [删除 PNP 文件](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [删除 PNP 文件夹](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [删除 PNP 列表项](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [删除 PNP 列表](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [删除 PNP 字段 (列)](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)