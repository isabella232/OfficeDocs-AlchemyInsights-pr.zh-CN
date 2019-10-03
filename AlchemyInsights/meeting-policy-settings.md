---
title: 会议策略设置
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: dac06690b51459ca166c15a5ef0f4c7e7a6d36f0
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376532"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="6181a-102">在 Microsoft 团队中管理会议策略</span><span class="sxs-lookup"><span data-stu-id="6181a-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="6181a-103">会议策略用于控制会议参与者对组织中的用户安排的会议参与者可用的功能。</span><span class="sxs-lookup"><span data-stu-id="6181a-103">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="6181a-104">会议策略的某些功能可能未在团队管理中心中实施（这些功能在文档中被标记为 "即将推出"）。</span><span class="sxs-lookup"><span data-stu-id="6181a-104">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="6181a-105">在这种情况下，或者如果遇到类似 "我们现在无法更新策略，但稍后再试一次" 这一错误（在 Microsoft 团队管理中心，我们建议使用 PowerShell 创建或修改团队会议策略。</span><span class="sxs-lookup"><span data-stu-id="6181a-105">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="6181a-106">有关会议策略的详细信息，请参阅以下资源：</span><span class="sxs-lookup"><span data-stu-id="6181a-106">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="6181a-107">若要了解如何创建策略、进行更改以及将用户分配到策略，请参阅[在团队中管理会议策略](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)。</span><span class="sxs-lookup"><span data-stu-id="6181a-107">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="6181a-108">若要使用 PowerShell cmdlet 进行策略更改，请参阅[团队 PowerShell 概述](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)。</span><span class="sxs-lookup"><span data-stu-id="6181a-108">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="6181a-109">您需要使用[Skype For Business PowerShell 模块](https://www.microsoft.com/download/details.aspx?id=39366)获取团队会议策略。</span><span class="sxs-lookup"><span data-stu-id="6181a-109">You need to use the [Skype for Business PowerShell module](https://www.microsoft.com/download/details.aspx?id=39366) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="6181a-110">有关详细信息，请参阅[\*-CsTeamsMeetingPolicy cmdlet 文档](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)。</span><span class="sxs-lookup"><span data-stu-id="6181a-110">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

<span data-ttu-id="6181a-111">**注意：** 可能需要长达24小时才能使策略更改对用户生效。</span><span class="sxs-lookup"><span data-stu-id="6181a-111">**Note:** It can take up to 24 hours for policy changes to take effect for users.</span></span> <span data-ttu-id="6181a-112">您可能无法立即对新创建的策略进行更改。等待4小时，并再次尝试修改新创建的策略。</span><span class="sxs-lookup"><span data-stu-id="6181a-112">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span> <span data-ttu-id="6181a-113">如果仍有问题，请尝试 PowerShell。</span><span class="sxs-lookup"><span data-stu-id="6181a-113">If you're still having problems, try PowerShell.</span></span>  