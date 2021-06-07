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
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783137"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="07fa4-102">管理网络研讨会注册</span><span class="sxs-lookup"><span data-stu-id="07fa4-102">Manage webinar registration</span></span>

<span data-ttu-id="07fa4-103">你可以通过使用 Teams PowerShell 命令管理谁可以注册 Teams 网络研讨会。</span><span class="sxs-lookup"><span data-stu-id="07fa4-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="07fa4-104">要安装 Teams Powershell，请参阅 [Teams PowerShell](/microsoftteams/teams-powershell-install)。</span><span class="sxs-lookup"><span data-stu-id="07fa4-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="07fa4-105">默认情况下，*WhoCanRegister* 处于启用状态，并已设置为“**EveryoneInCompany**”。</span><span class="sxs-lookup"><span data-stu-id="07fa4-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="07fa4-106">要允许任何人（包括匿名用户）注册，必须通过使用以下 PowerShell 命令将会议策略设置为 **所有人**：</span><span class="sxs-lookup"><span data-stu-id="07fa4-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="07fa4-107">**注意**：如果在会议设置中关闭了匿名加入，则匿名用户将无法加入网络研讨会。</span><span class="sxs-lookup"><span data-stu-id="07fa4-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="07fa4-108">要了解并启用此设置，请参阅 [管理 Microsoft Teams 中的会议设置](/microsoftteams/meeting-settings-in-teams)。</span><span class="sxs-lookup"><span data-stu-id="07fa4-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="07fa4-109">如果要关闭会议注册，请将 *AllowMeetingRegistration* 设置为 **False**。</span><span class="sxs-lookup"><span data-stu-id="07fa4-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="07fa4-110">要了解关于配置谁可以注册网络研讨会的详细信息，请参阅 [配置谁可以注册网络研讨会](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)。</span><span class="sxs-lookup"><span data-stu-id="07fa4-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="07fa4-111">有关 Microsoft Lists 设置的详细信息，请参阅 [Microsoft Lists 的控制设置](/sharepoint/control-lists)。</span><span class="sxs-lookup"><span data-stu-id="07fa4-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
