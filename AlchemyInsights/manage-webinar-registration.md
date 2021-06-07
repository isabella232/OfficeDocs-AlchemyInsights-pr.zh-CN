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
ms.openlocfilehash: 988e97896cc1000c11ce1e81cd169090b1c39104
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760823"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="d3cb2-102">管理网络研讨会注册</span><span class="sxs-lookup"><span data-stu-id="d3cb2-102">Manage webinar registration</span></span>

<span data-ttu-id="d3cb2-103">你可以通过使用 Teams PowerShell 命令管理谁可以注册 Teams 网络研讨会。</span><span class="sxs-lookup"><span data-stu-id="d3cb2-103">You can manage who can register for Teams Webinars by using Teams PowerShell commands.</span></span> <span data-ttu-id="d3cb2-104">默认情况下，*WhoCanRegister* 处于启用状态，并已设置为“**所有人**”。</span><span class="sxs-lookup"><span data-stu-id="d3cb2-104">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="d3cb2-105">如果要关闭会议注册，请将 *AllowMeetingRegistration* 设置为 **False**。</span><span class="sxs-lookup"><span data-stu-id="d3cb2-105">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="d3cb2-106">要更改这些设置，必须安装 [Teams PowerShell](/microsoftteams/teams-powershell-install)。</span><span class="sxs-lookup"><span data-stu-id="d3cb2-106">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="d3cb2-107">并将对 Teams 网络研讨会强制实施会议策略。</span><span class="sxs-lookup"><span data-stu-id="d3cb2-107">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="d3cb2-108">例如，如果在会议设置中关闭了匿名加入，则匿名用户将无法加入网络研讨会。</span><span class="sxs-lookup"><span data-stu-id="d3cb2-108">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="d3cb2-109">要了解关于配置谁可以注册网络研讨会的详细信息，请参阅 [配置谁可以注册网络研讨会](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)。</span><span class="sxs-lookup"><span data-stu-id="d3cb2-109">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="d3cb2-110">有关 Microsoft Lists 设置的详细信息，请参阅 [Microsoft Lists 的控制设置](/sharepoint/control-lists)。</span><span class="sxs-lookup"><span data-stu-id="d3cb2-110">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>