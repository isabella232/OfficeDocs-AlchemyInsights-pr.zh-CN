---
title: 从 Office 安装中卸载或排除 Teams
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2662"
- "9000660"
ms.openlocfilehash: 2d96d54cb479f5f52cc707d4307cf9cf1e891a01
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827782"
---
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a>从新的或现有的 Office 安装中卸载或排除 Teams

Microsoft Teams 包含在 Microsoft 365 企业应用版、Microsoft 365 商业应用版和 Office for Mac。

- 使用 [Office 部署工具](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) 将 Teams 从 Office 的新安装中排除。
- 若要 *从运行* Windows 的设备卸载 Teams，请参阅 [卸载 Microsoft Teams。](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) 若要从多个目标计算机或用户清理 Microsoft Teams，请参阅 [Microsoft Teams 部署清理](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)。
- 使用 [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) 选项可防止 Microsoft Teams 随 Office 一起自动安装。
- 在安装 *Teams* 之前，使用 [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)选项可防止 Microsoft Teams 在安装后自动启动。

如果你使用的是 Microsoft Office for Mac，请参阅 Mac [上的 Microsoft Teams 安装](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)。