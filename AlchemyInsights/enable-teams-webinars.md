---
title: 启用 Teams 网络研讨会
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760827"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="186ea-102">启用 Teams 网络研讨会</span><span class="sxs-lookup"><span data-stu-id="186ea-102">Enable Teams Webinars</span></span>

<span data-ttu-id="186ea-103">默认情况下启用网络研讨会。</span><span class="sxs-lookup"><span data-stu-id="186ea-103">Webinars are enabled by default.</span></span> <span data-ttu-id="186ea-104">可以通过使用 Teams PowerShell 命令来管理谁可以安排和注册 Teams 网络研讨会。</span><span class="sxs-lookup"><span data-stu-id="186ea-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="186ea-105">所有可以创建会议的用户也可以创建网上研讨会会议。</span><span class="sxs-lookup"><span data-stu-id="186ea-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="186ea-106">如果要管理谁可以安排团队网络研讨会，请使用 *AllowMeetingRegistration*。</span><span class="sxs-lookup"><span data-stu-id="186ea-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="186ea-107">默认情况下，*WhoCanRegister* 处于启用状态，并已设置为“**所有人**”。</span><span class="sxs-lookup"><span data-stu-id="186ea-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="186ea-108">如果要关闭会议注册，请将 *AllowMeetingRegistration* 设置为 **False**。</span><span class="sxs-lookup"><span data-stu-id="186ea-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="186ea-109">要更改这些设置，必须安装 [Teams PowerShell](/microsoftteams/teams-powershell-install)。</span><span class="sxs-lookup"><span data-stu-id="186ea-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="186ea-110">并将对 Teams 网络研讨会强制实施会议策略。</span><span class="sxs-lookup"><span data-stu-id="186ea-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="186ea-111">例如，如果在会议设置中关闭了匿名加入，则匿名用户将无法加入网络研讨会。</span><span class="sxs-lookup"><span data-stu-id="186ea-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="186ea-112">要了解关于配置谁可以注册网络研讨会的详细信息，请参阅 [配置谁可以注册网络研讨会](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)。</span><span class="sxs-lookup"><span data-stu-id="186ea-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="186ea-113">有关 Microsoft Lists 设置的详细信息，请参阅 [Microsoft Lists 的控制设置](/sharepoint/control-lists)。</span><span class="sxs-lookup"><span data-stu-id="186ea-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>