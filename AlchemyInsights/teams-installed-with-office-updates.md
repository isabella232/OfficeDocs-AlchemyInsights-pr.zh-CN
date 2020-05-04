---
title: 使用 Office 更新安装的团队
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2599"
- "9000140"
- "9000660"
- "2509"
ms.openlocfilehash: ddb9ffb2f6545e99a593ee830854f986438950cd
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010820"
---
# <a name="microsoft-teams-installed-with-office-updates"></a><span data-ttu-id="f5d7b-102">安装了 Office 更新的 Microsoft 团队</span><span class="sxs-lookup"><span data-stu-id="f5d7b-102">Microsoft Teams installed with Office updates</span></span>

<span data-ttu-id="f5d7b-103">Microsoft 团队作为 Microsoft 365 Apps for enterprise、Microsoft 365 Apps for business 和 Office for Mac 的***全新安装***的一部分包括在内。</span><span class="sxs-lookup"><span data-stu-id="f5d7b-103">Microsoft Teams is included as part of ***new installations*** of Microsoft 365 Apps for enterprise, Microsoft 365 Apps for business, and Office for Mac.</span></span> <span data-ttu-id="f5d7b-104">有关详细信息，请参阅[何时 Microsoft 团队何时开始将新安装的 Office？](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)</span><span class="sxs-lookup"><span data-stu-id="f5d7b-104">For more information, see [When will Microsoft Teams start being included with new installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)</span></span>

<span data-ttu-id="f5d7b-105">此外，从每月频道中的版本1906开始，在将现有安装更新到最新版本时，团队将逐步添加到运行 Windows 的 Microsoft 365 应用程序的***现有安装***（以及 Microsoft 365 应用程序）。</span><span class="sxs-lookup"><span data-stu-id="f5d7b-105">Additionally, starting with Version 1906 in Monthly Channel, Teams will gradually be added to ***existing installations*** of Microsoft 365 Apps for enterprise (and Microsoft 365 Apps for business) on devices running Windows when you update your existing installation to the latest version.</span></span> <span data-ttu-id="f5d7b-106">有关详细信息，请参阅[现有安装的 Office？](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)</span><span class="sxs-lookup"><span data-stu-id="f5d7b-106">For more information, see [What about existing installations of Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)</span></span>

<span data-ttu-id="f5d7b-107">**注意：** 如果您不想等待此首展计划，可以按照[这些说明](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)将团队部署为独立用户，也可以让您的用户自行安装团队https://teams.microsoft.com/downloads。</span><span class="sxs-lookup"><span data-stu-id="f5d7b-107">**Note:** If you don't want to wait for this rollout schedule, you can deploy Teams as standalone for your users by [following these instructions](https://docs.microsoft.com/MicrosoftTeams/msi-deployment), or you can have your users install Teams for themselves from https://teams.microsoft.com/downloads.</span></span>

<span data-ttu-id="f5d7b-108">如果你的组织未准备好部署团队，则可以从 Office 的[新](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps)安装或[现有](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams)安装中***排除团队***。</span><span class="sxs-lookup"><span data-stu-id="f5d7b-108">If your organization isn't ready to deploy Teams, you can ***exclude Teams*** from [new](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) or [existing](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) installations of Office.</span></span> <span data-ttu-id="f5d7b-109">如果您希望安装团队，但不希望团队在安装后自动为用户启动，请参阅 "[阻止 Microsoft 团队在安装后自动](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)启动"。</span><span class="sxs-lookup"><span data-stu-id="f5d7b-109">If you want Teams to be installed, but don't want Teams to start automatically for the user after it's installed, see [Prevent Microsoft Teams from starting automatically after installation](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation).</span></span>

<span data-ttu-id="f5d7b-110">若要从运行 Windows 的设备中***卸载团队***，请参阅[卸载 Microsoft 团队](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81)。</span><span class="sxs-lookup"><span data-stu-id="f5d7b-110">To ***uninstall Teams*** from a device running Windows, see [Uninstall Microsoft Teams](https://support.office.com/article/uninstall-microsoft-teams-3b159754-3c26-4952-abe7-57d27f5f4c81).</span></span> <span data-ttu-id="f5d7b-111">若要从多个目标计算机或用户清理 Microsoft 团队，请参阅[Microsoft 团队部署清理](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up)。</span><span class="sxs-lookup"><span data-stu-id="f5d7b-111">To clean up Microsoft Teams from multiple target machines or users, see [Microsoft Teams deployment cleanup](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).</span></span>

<span data-ttu-id="f5d7b-112">如果使用的是共享计算机、远程桌面服务（RDS）或虚拟桌面基础结构（VDI），请参阅[与 Microsoft 团队共享的计算机和 VDI 环境](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams)。</span><span class="sxs-lookup"><span data-stu-id="f5d7b-112">If you're using shared computers, Remote Desktop Services (RDS), or Virtual Desktop Infrastructure (VDI), see [Shared computer and VDI environments with Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).</span></span> <span data-ttu-id="f5d7b-113">如果使用的是 Office for Mac，请参阅[mac 上的 Microsoft 团队安装](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac)。</span><span class="sxs-lookup"><span data-stu-id="f5d7b-113">If you're using Office for Mac, see [Microsoft Teams installations on a Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).</span></span>

<span data-ttu-id="f5d7b-114">**注意：** 团队安装完成后，每两周[都会自动更新](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams)一次，并提供新的功能和质量更新。</span><span class="sxs-lookup"><span data-stu-id="f5d7b-114">**Note:** After Teams is installed, it's [automatically updated](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) approximately every two weeks with new features and quality updates.</span></span> 