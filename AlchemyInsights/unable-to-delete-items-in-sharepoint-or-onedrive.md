---
title: 无法删除项目或SharePoint OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 3601c5eff121e10b6bddace6f7228204a01080a636e24f3a56373fe8d469c799
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038507"
---
# <a name="unable-to-delete-items"></a>无法删除项目

- 保留策略可能会导致此问题，您需要禁用或排除导致此问题各自的保留。 删除保留策略或保留后，更改最多可能需要 24 小时才能生效。 确保项目上没有 [保留](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) 策略设置。

- 网站可能超出了存储限制，增加了 [网站配额并](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) 删除了项目。

- 确保该项目未 [签出给](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) 其他用户。

- 最后，管理员可以使用[SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) 其中包含一个 PowerShell 命令库，允许您执行复杂的管理操作，如强制删除购买项目。
- [删除 PNP 文件](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [删除 PNP 文件夹](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [删除 PNP 列表项](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [删除 PNP 列表](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [删除"PNP 字段 (列) ](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)