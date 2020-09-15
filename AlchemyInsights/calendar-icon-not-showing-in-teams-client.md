---
title: Teams 客户端不显示日历图标
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: f30cd5bda62756cf6b912ed150b4e59e7ca4d85d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684688"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="9e360-102">Teams 客户端不显示日历图标</span><span class="sxs-lookup"><span data-stu-id="9e360-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="9e360-103">Teams 中的日历选项卡需要通过 Exchange Web 服务访问 Exchange 邮箱。</span><span class="sxs-lookup"><span data-stu-id="9e360-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="9e360-104">Exchange 邮箱可以是 Online 版或本地版。</span><span class="sxs-lookup"><span data-stu-id="9e360-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="9e360-105">如果 Online 版用户未看到日历选项卡，请确保用户已[获得 Exchange Online 邮箱许可证并启用该邮箱](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)。</span><span class="sxs-lookup"><span data-stu-id="9e360-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="9e360-106">若用户拥有有效的 Exchange Online 邮箱，但仍然看不到日历选项卡，则可能出现了网络问题。</span><span class="sxs-lookup"><span data-stu-id="9e360-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="9e360-107">使用 [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) 并对受影响的相应用户运行 **Microsoft Exchange Web 服务连接测试**。</span><span class="sxs-lookup"><span data-stu-id="9e360-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="9e360-108">最后检查 [Teams 应用 – 应用设置策略](https://admin.teams.microsoft.com/policies/app-setup)，确保未从应用到该用户的策略中删除日历应用（最有可能是“全局(默认为组织范围)”）\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="9e360-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="9e360-109">若用户托管在本地，你需要确认混合配置正常。</span><span class="sxs-lookup"><span data-stu-id="9e360-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="9e360-110">请使用[混合配置向导](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)排除故障。</span><span class="sxs-lookup"><span data-stu-id="9e360-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="9e360-111">请注意，[Teams 需要 Exchange 2016 CU3 或更高版本](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)。</span><span class="sxs-lookup"><span data-stu-id="9e360-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
