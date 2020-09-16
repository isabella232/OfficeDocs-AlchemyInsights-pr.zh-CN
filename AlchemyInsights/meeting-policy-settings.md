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
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794324"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="ed2fe-102">在 Microsoft 团队中管理会议策略</span><span class="sxs-lookup"><span data-stu-id="ed2fe-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="ed2fe-103">**注意：最长可能需要24小时才能使策略更改对用户生效。**</span><span class="sxs-lookup"><span data-stu-id="ed2fe-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="ed2fe-104">您可能无法立即对新创建的策略进行更改。等待4小时，并再次尝试修改新创建的策略。</span><span class="sxs-lookup"><span data-stu-id="ed2fe-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="ed2fe-105">会议策略用于控制会议参与者对组织中的用户安排的会议参与者可用的功能。</span><span class="sxs-lookup"><span data-stu-id="ed2fe-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="ed2fe-106">会议策略的某些功能可能未在团队管理中心中实施，但 (这些功能在文档) 中标记为 "即将推出"。</span><span class="sxs-lookup"><span data-stu-id="ed2fe-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="ed2fe-107">在这种情况下，或者如果遇到类似 "我们现在无法更新策略，但稍后再试一次" 这一错误（在 Microsoft 团队管理中心，我们建议使用 PowerShell 创建或修改团队会议策略。</span><span class="sxs-lookup"><span data-stu-id="ed2fe-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="ed2fe-108">有关会议策略的详细信息，请参阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="ed2fe-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="ed2fe-109">若要了解如何创建策略、进行更改以及将用户分配到策略，请参阅 [在团队中管理会议策略](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)。</span><span class="sxs-lookup"><span data-stu-id="ed2fe-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="ed2fe-110">若要使用 PowerShell cmdlet 进行策略更改，请参阅 [团队 PowerShell 概述](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)。</span><span class="sxs-lookup"><span data-stu-id="ed2fe-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="ed2fe-111">您需要使用 [Skype For Business PowerShell 模块](https://www.microsoft.com/download/details.aspx?id=39366) 获取团队会议策略。</span><span class="sxs-lookup"><span data-stu-id="ed2fe-111">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="ed2fe-112">有关详细信息，请参阅 [\*-CsTeamsMeetingPolicy cmdlet 文档](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) 。</span><span class="sxs-lookup"><span data-stu-id="ed2fe-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

