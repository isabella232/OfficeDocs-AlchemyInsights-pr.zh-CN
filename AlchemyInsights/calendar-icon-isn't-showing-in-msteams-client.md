---
title: 日历图标在 Microsoft 团队客户端中未显示
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "6794"
- "3403"
ms.openlocfilehash: e28b1c8d5d0feef1a743c8527db424af4c205fe9
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576378"
---
# <a name="calendar-icon-isnt-showing-in-microsoft-teams-client"></a><span data-ttu-id="717f7-102">日历图标在 Microsoft 团队客户端中未显示</span><span class="sxs-lookup"><span data-stu-id="717f7-102">Calendar icon isn't showing in Microsoft Teams client</span></span>

<span data-ttu-id="717f7-103">团队中的 " **日历** " 选项卡需要通过 Exchange Web 服务访问 exchange 邮箱。</span><span class="sxs-lookup"><span data-stu-id="717f7-103">The **Calendar** Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="717f7-104">Exchange 邮箱可以是联机的，也可以是本地的。</span><span class="sxs-lookup"><span data-stu-id="717f7-104">The Exchange mailbox can be Online, or On-Premises.</span></span> <span data-ttu-id="717f7-105">对于看不到 " **日历** " 选项卡的联机用户，请确保他们已 [获得 Exchange Online 邮箱许可，并且已启用邮箱](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes)。</span><span class="sxs-lookup"><span data-stu-id="717f7-105">For Online users who do not see the **Calendar** Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span> <span data-ttu-id="717f7-106">如果您的用户驻留在本地，则需要确认您的混合配置运行状况良好。</span><span class="sxs-lookup"><span data-stu-id="717f7-106">If your users are homed On-Premises, you need to confirm that your Hybrid configuration is healthy.</span></span> <span data-ttu-id="717f7-107">请使用[混合配置向导](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent)排除故障。</span><span class="sxs-lookup"><span data-stu-id="717f7-107">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span> <span data-ttu-id="717f7-108">请注意，[Teams 需要 Exchange 2016 CU3 或更高版本](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)。</span><span class="sxs-lookup"><span data-stu-id="717f7-108">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>

<span data-ttu-id="717f7-109">有关详细信息和疑难解答步骤，请参阅 [Microsoft 团队和 Exchange Server 交互问题的疑难解答](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue)。</span><span class="sxs-lookup"><span data-stu-id="717f7-109">For more information and troubleshooting steps, see [Troubleshoot Microsoft Teams and Exchange Server interaction issues](https://docs.microsoft.com/microsoftteams/troubleshoot/known-issues/teams-exchange-interaction-issue).</span></span>
