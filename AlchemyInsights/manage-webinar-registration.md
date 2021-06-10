---
title: 管理网络研讨会注册
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: 0db6f434fa74970ac6083501ab26762cc6b7885f
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798634"
---
# <a name="manage-webinar-registration"></a>管理网络研讨会注册

你可以通过使用 Teams PowerShell 命令管理谁可以注册 Teams 网络研讨会。 要安装 Teams Powershell，请参阅 [Teams PowerShell](/microsoftteams/teams-powershell-install)。 

默认情况下，*WhoCanRegister* 处于启用状态，并已设置为“**所有人**”。 

如果在会议邀请中未看到允许所有人注册的选项，请重新运行设置 *WhoCanRegister* 为所有人，然后等待 24 小时。 要重新运行 *WhoCanRegister*，请使用 Powershell 命令：

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**注意**：如果在会议设置中关闭了匿名加入，则匿名用户将无法加入网络研讨会。 要了解并启用此设置，请参阅 [管理 Microsoft Teams 中的会议设置](/microsoftteams/meeting-settings-in-teams)。

如果要关闭会议注册，请将 *AllowMeetingRegistration* 设置为 **False**。

要了解关于配置谁可以注册网络研讨会的详细信息，请参阅 [配置谁可以注册网络研讨会](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)。 有关 Microsoft Lists 设置的详细信息，请参阅 [Microsoft Lists 的控制设置](/sharepoint/control-lists)。
