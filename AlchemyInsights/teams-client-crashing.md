---
title: Teams 客户端崩溃
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: a292e160abcfc26ffebc454d32ee489a319a23f4bb81e70fe5dbe72bfd0b8b81
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890328"
---
# <a name="teams-client-crashing"></a>Teams 客户端崩溃

如果 Teams 客户端发生了故障，请尝试执行以下操作：

- 如果使用的是 Teams 桌面应用，请[确保应用已完全更新](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。

- 确保所有 [Microsoft 365 URL 和地址范围](https://docs.microsoft.com/microsoftteams/connectivity-issues)均可访问。

- 使用租户管理员帐户登录，然后检查[服务运行状况仪表板](https://docs.microsoft.com/office365/enterprise/view-service-health)，以确认没有任何故障或服务降级。

- 卸载并重新安装 Teams 应用程序
    - 浏览到计算机上的 %appdata%\Microsoft\Teams\ 文件夹，然后删除该目录中的所有文件。
    - [下载并安装 Teams 应用](https://www.microsoft.com/microsoft-teams/download-app)，如有可能，请以管理员身份安装 Teams（右键单击 Teams 安装程序，然后选择“**以管理员身份运行**”(如果有)）。

如果 Teams 客户端仍然崩溃，请尝试重现此问题。如果可以，请执行以下操作：

1. 请使用步骤记录器捕获步骤。
    - 关闭所有不必要的或机密的应用程序。
    - 启动步骤记录器并在使用受影响的用户帐户登录时重现该问题。
    - [收集捕获记录的重现步骤的 Teams 日志](https://docs.microsoft.com/microsoftteams/log-files)。 **注意**：请确保捕获受影响用户的登录地址。
    - 收集转储和/或故障存储桶信息 (Windows)。在发生崩溃的计算机上启动 Windows Powershell，然后运行以下命令（在每个命令之后按 Enter）：

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. 生成文本文件并显示在屏幕上后，保存该文件并将其附加到服务请求。 
