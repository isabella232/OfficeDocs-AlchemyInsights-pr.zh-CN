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
# <a name="manage-webinar-registration"></a><span data-ttu-id="cd9c9-102">管理网络研讨会注册</span><span class="sxs-lookup"><span data-stu-id="cd9c9-102">Manage webinar registration</span></span>

<span data-ttu-id="cd9c9-103">你可以通过使用 Teams PowerShell 命令管理谁可以注册 Teams 网络研讨会。</span><span class="sxs-lookup"><span data-stu-id="cd9c9-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="cd9c9-104">要安装 Teams Powershell，请参阅 [Teams PowerShell](/microsoftteams/teams-powershell-install)。</span><span class="sxs-lookup"><span data-stu-id="cd9c9-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="cd9c9-105">默认情况下，*WhoCanRegister* 处于启用状态，并已设置为“**所有人**”。</span><span class="sxs-lookup"><span data-stu-id="cd9c9-105">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> 

<span data-ttu-id="cd9c9-106">如果在会议邀请中未看到允许所有人注册的选项，请重新运行设置 *WhoCanRegister* 为所有人，然后等待 24 小时。</span><span class="sxs-lookup"><span data-stu-id="cd9c9-106">If you don't see the option to allow registration for Everyone in the meeting invitation, rerun setting *WhoCanRegister* to Everyone and wait 24 hours.</span></span> <span data-ttu-id="cd9c9-107">要重新运行 *WhoCanRegister*，请使用 Powershell 命令：</span><span class="sxs-lookup"><span data-stu-id="cd9c9-107">To rerun *WhoCanRegister*, use the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="cd9c9-108">**注意**：如果在会议设置中关闭了匿名加入，则匿名用户将无法加入网络研讨会。</span><span class="sxs-lookup"><span data-stu-id="cd9c9-108">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="cd9c9-109">要了解并启用此设置，请参阅 [管理 Microsoft Teams 中的会议设置](/microsoftteams/meeting-settings-in-teams)。</span><span class="sxs-lookup"><span data-stu-id="cd9c9-109">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="cd9c9-110">如果要关闭会议注册，请将 *AllowMeetingRegistration* 设置为 **False**。</span><span class="sxs-lookup"><span data-stu-id="cd9c9-110">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="cd9c9-111">要了解关于配置谁可以注册网络研讨会的详细信息，请参阅 [配置谁可以注册网络研讨会](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)。</span><span class="sxs-lookup"><span data-stu-id="cd9c9-111">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="cd9c9-112">有关 Microsoft Lists 设置的详细信息，请参阅 [Microsoft Lists 的控制设置](/sharepoint/control-lists)。</span><span class="sxs-lookup"><span data-stu-id="cd9c9-112">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
