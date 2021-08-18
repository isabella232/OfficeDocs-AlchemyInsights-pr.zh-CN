---
title: 将Teams部署为独立安装，或部署新的或现有的Office安装
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 6425b1eac3d5c99a6dfd227a1b445412c51a39b8
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320112"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>将Teams部署为独立安装，或部署新的或现有的Office安装

Microsoft Teams现在作为新安装的 Microsoft 365 企业应用版、Microsoft 365 商业应用版和 Office for Mac 的一Office for Mac。 有关详细信息，请参阅何时Microsoft Teams新安装的[Office？](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

此外，从当前频道的版本 1906 开始，当你将现有安装更新到最新版本时，Teams 将添加到运行 Windows 的设备上 Microsoft 365 企业应用版 (和 Microsoft 365 商业应用版) 的现有安装中。 有关详细信息，请参阅[What about existing installations of Office？](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

**注意**：如果不想等待此推出计划，可以按照以下说明为用户将 Teams 部署为独立部署，也可以让用户从 [](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)自行安装 Teams。 [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)

如果你的组织尚未准备好部署 Teams，我们可采取一些步骤，Teams安装或现有安装的 Office。  [](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) [](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) 如果要Teams，但不希望 Teams安装后自动为用户启动，请参阅防止 Microsoft Teams 在安装后[自动启动](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)。

若要 ***从Teams*** 的设备上卸载Windows，请参阅卸载 [Microsoft Teams。](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81) 若要清理Microsoft Teams计算机或用户的部署，请参阅Microsoft Teams[清理。](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)

如果你使用的是共享计算机、远程桌面服务 (RDS) 或虚拟桌面基础结构 (VDI) ，请参阅使用 Microsoft Teams 的共享[计算机和 VDI 环境](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)。

如果你使用的是 Office for Mac，请参阅[Microsoft Teams Mac 上的安装](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)。

**注意**：Teams后，大约每两周自动更新一次新功能 [](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams)和质量更新。 