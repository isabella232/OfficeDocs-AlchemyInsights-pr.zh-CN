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
# <a name="uninstall-or-exclude-teams-from-new-or-existing-office-installations"></a><span data-ttu-id="cd3ad-102">从新的或现有的 Office 安装中卸载或排除 Teams</span><span class="sxs-lookup"><span data-stu-id="cd3ad-102">Uninstall or exclude Teams from new or existing Office installations</span></span>

<span data-ttu-id="cd3ad-103">Microsoft Teams 包含在 Microsoft 365 企业应用版、Microsoft 365 商业应用版和 Office for Mac。</span><span class="sxs-lookup"><span data-stu-id="cd3ad-103">Microsoft Teams is included as part of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span>

- <span data-ttu-id="cd3ad-104">使用 [Office 部署工具](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) 将 Teams 从 Office 的新安装中排除。</span><span class="sxs-lookup"><span data-stu-id="cd3ad-104">Use the [Office Deployment Tool](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) to exclude Teams from new installations of Office.</span></span>
- <span data-ttu-id="cd3ad-105">若要 *从运行* Windows 的设备卸载 Teams，请参阅 [卸载 Microsoft Teams。](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81)</span><span class="sxs-lookup"><span data-stu-id="cd3ad-105">To *uninstall* Teams from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="cd3ad-106">若要从多个目标计算机或用户清理 Microsoft Teams，请参阅 [Microsoft Teams 部署清理](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)。</span><span class="sxs-lookup"><span data-stu-id="cd3ad-106">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment clean up](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>
- <span data-ttu-id="cd3ad-107">使用 [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) 选项可防止 Microsoft Teams 随 Office 一起自动安装。</span><span class="sxs-lookup"><span data-stu-id="cd3ad-107">Use the [PreventTeamsInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams
) option to prevent Microsoft Teams from installing automatically with Office.</span></span>
- <span data-ttu-id="cd3ad-108">在安装 *Teams* 之前，使用 [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)选项可防止 Microsoft Teams 在安装后自动启动。</span><span class="sxs-lookup"><span data-stu-id="cd3ad-108">Use the [PreventFirstLaunchAfterInstall](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation) option, *before Teams is installed*, to prevent Microsoft Teams from starting automatically after installation.</span></span>

<span data-ttu-id="cd3ad-109">如果你使用的是 Microsoft Office for Mac，请参阅 Mac [上的 Microsoft Teams 安装](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)。</span><span class="sxs-lookup"><span data-stu-id="cd3ad-109">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>