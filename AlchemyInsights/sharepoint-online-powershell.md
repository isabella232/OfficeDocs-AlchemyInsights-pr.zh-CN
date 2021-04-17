---
title: Sharepoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 839a70282b4dd619e9dbe8167ef0e409e468b1ad
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830572"
---
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

在 Sharepoint Online 中使用 PowerShell 或脚本 有关详细信息，请访问以下链接。
- [SharePoint Online 命令行管理程序入门](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [通过多重身份验证和 MFA (SPO PowerShell) ](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint Patterns and Practices (PnP) ](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions to SPO.

> [!NOTE]
> - 如果在与 SPO 命令行管理程序连接时遇到问题，请确保已更新到最新版本，并尝试使用 *"Import-Module Microsoft.Online.SharePoint.PowerShell"* 重新导入模块。 [](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1)
> - 如果您尝试运行客户端对象模型脚本，则需要在本地计算机上安装[Sharepoint Online 客户端组件 SDK。](https://www.microsoft.com/download/details.aspx?id=42038)
> - 如果在从 PowerShell 运行脚本时遇到问题，可能需要考虑以管理员角色运行 PowerShell 并更改 [执行策略](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)。