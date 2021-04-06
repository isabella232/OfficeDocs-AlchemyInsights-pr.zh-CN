---
title: 识别 Windows 虚拟桌面问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590265"
---
# <a name="identify-windows-virtual-desktop-issues"></a>识别 Windows 虚拟桌面问题

Windows 虚拟桌面诊断仅使用一个 PowerShell cmdlet，但包含许多可选参数，可帮助缩小和隔离问题。 首先，请执行以下操作： 

1. 下载并导入 Windows Virtual Desktop PowerShell 模块。 有关详细信息，请参阅 [用于 Windows PowerShell 的 Windows Virtual Desktop cmdlet](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)。

1. 运行以下 cmdlet 登录你的帐户：
    
    示例：`Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**注意：** PowerShell 的所有查询都必须包含 -UserName 或 -ActivityID 参数。 有关监视功能的信息，请参阅将 [日志分析用于诊断功能](https://go.microsoft.com/fwlink/?linkid=2126847)。

若要按用户筛选诊断活动，请运行以下 cmdlet：

示例：`Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

你可以运行一系列筛选器来诊断问题。 若要深入了解如何诊断问题，请参阅 [识别并诊断 Windows Virtual Desktop 问题](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)。

若要了解有关常见错误的详细信息，请参阅 [错误发现](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios)。
