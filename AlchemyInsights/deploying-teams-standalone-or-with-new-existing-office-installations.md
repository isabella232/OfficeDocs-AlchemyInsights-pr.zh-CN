---
title: 将团队部署为独立或使用新的或现有 Office 安装
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: 5ec5277a758fc5171c846266787c2fbcf751f21c
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617885"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>将团队部署为独立或使用新的或现有 Office 安装

Microsoft 团队现已作为 Microsoft 365 应用程序的***新安装***的一部分、microsoft 365 商业版应用程序和 Office for Mac 包括在内。 有关详细信息，请参阅[何时 Microsoft 团队何时开始将新安装的 Office？](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

此外，从当前通道中的版本1906开始，在将现有安装更新到最新版本时，会将团队添加到运行 Windows 的 Microsoft 365 应用程序的***现有安装***（以及 Microsoft 365 应用程序）。 有关详细信息，请参阅[现有安装的 Office？](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> 如果您不想等待此首展计划，可以按照[这些说明](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)将团队部署为独立用户，   也可以让您的用户自行安装团队  [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads) 。

如果您的组织未准备好部署团队，则可以使用从[新](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps)的或[现有](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams)的 Office 安装中***排除团队***所需的步骤。 如果您希望安装团队，但不希望团队在安装后自动为用户启动，请参阅 "[阻止 Microsoft 团队在安装后自动](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)启动"。

若要从运行 Windows 的设备中***卸载团队***，请参阅[卸载 Microsoft 团队](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)。 若要从多个目标计算机或用户清理 Microsoft 团队，请参阅[Microsoft 团队部署清理](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)。

如果使用的是共享计算机、远程桌面服务（RDS）或虚拟桌面基础结构（VDI），请参阅[与 Microsoft 团队共享的计算机和 VDI 环境](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)。

如果使用的是 Office for Mac，请参阅[mac 上的 Microsoft 团队安装](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)。

> [!NOTE]
> 团队安装完成后，每两周[都会自动更新](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams)一次，并提供新的功能和质量更新。 