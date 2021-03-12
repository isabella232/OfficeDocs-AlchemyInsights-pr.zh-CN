---
title: 会议策略设置
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704596"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="26da8-102">在 Microsoft Teams 中管理会议策略</span><span class="sxs-lookup"><span data-stu-id="26da8-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="26da8-103">**注意：策略更改最多可能需要 24 小时才能对用户生效。**</span><span class="sxs-lookup"><span data-stu-id="26da8-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="26da8-104">可能无法立即对新创建的策略进行更改;请等待 4 小时，然后再次尝试修改新创建的策略。</span><span class="sxs-lookup"><span data-stu-id="26da8-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="26da8-105">会议策略用于控制对组织中用户安排的会议的会议参与者可用的功能。</span><span class="sxs-lookup"><span data-stu-id="26da8-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="26da8-106">会议策略的一些功能可能尚未在 Teams 管理中心实现 (这些功能在) 文档中标记为"即将) 。</span><span class="sxs-lookup"><span data-stu-id="26da8-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="26da8-107">在这种情况下，或者如果你收到类似"我们现在无法更新策略，但稍后在 Microsoft Teams 管理中心重试"等错误，我们建议你使用 PowerShell 创建或修改 Teams 会议策略。</span><span class="sxs-lookup"><span data-stu-id="26da8-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="26da8-108">有关会议策略详细信息，请参阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="26da8-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="26da8-109">若要了解如何创建策略、进行更改以及向策略分配用户，请参阅["在 Teams 中管理会议策略"。](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="26da8-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="26da8-110">若要使用 PowerShell cmdlet 更改策略，请参阅 [Teams PowerShell 概述](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)。</span><span class="sxs-lookup"><span data-stu-id="26da8-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="26da8-111">你需要将 Skype [for Business PowerShell 模块用于](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) Teams 会议策略。</span><span class="sxs-lookup"><span data-stu-id="26da8-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="26da8-112">有关详细信息 [，请参阅 \*-CsTeamsMeetingPolicy cmdlet](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) 文档。</span><span class="sxs-lookup"><span data-stu-id="26da8-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

