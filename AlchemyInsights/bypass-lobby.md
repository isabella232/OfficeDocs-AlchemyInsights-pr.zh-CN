---
title: 旁路前厅浏览
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889072"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="19f49-102">控制团队中的前厅浏览设置和参与级别</span><span class="sxs-lookup"><span data-stu-id="19f49-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="19f49-103">如果您想要允许所有人（包括拨入、外部和匿名用户）**绕过会议厅**，请使用 PowerShell 来完成此任务。</span><span class="sxs-lookup"><span data-stu-id="19f49-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="19f49-104">下面的示例展示了如何修改组织的全局会议策略。</span><span class="sxs-lookup"><span data-stu-id="19f49-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="19f49-105">此 cmdlet 当前需要使用 Skype for Business PowerShell 模块。</span><span class="sxs-lookup"><span data-stu-id="19f49-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="19f49-106">若要设置为使用此 cmdlet，请[通过 PowerShell 来查看管理策略](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)。</span><span class="sxs-lookup"><span data-stu-id="19f49-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="19f49-107">设置完策略后，需要将其应用于用户;或者，如果您修改了全局策略，它将自动应用于用户。</span><span class="sxs-lookup"><span data-stu-id="19f49-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="19f49-108">对于任何策略更改，至少需要等待**4 小时长达24小时**才能使策略生效。</span><span class="sxs-lookup"><span data-stu-id="19f49-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="19f49-109">在进行这些更改之前，请务必查看下面的文档，以了解所允许的确切内容。</span><span class="sxs-lookup"><span data-stu-id="19f49-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="19f49-110">了解团队会议会议厅策略控件</span><span class="sxs-lookup"><span data-stu-id="19f49-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="19f49-111">这些设置控制哪些会议参与者在会议厅中等待，并在会议中允许他们参加会议和参与的程度。</span><span class="sxs-lookup"><span data-stu-id="19f49-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="19f49-112">您可以使用 PowerShell 更新团队管理中心中尚未实现的会议策略设置（标为 "即将推出"）。</span><span class="sxs-lookup"><span data-stu-id="19f49-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="19f49-113">有关允许所有用户绕过会议厅的 PowerShell cmdlet 示例，请参阅下面的示例。</span><span class="sxs-lookup"><span data-stu-id="19f49-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="19f49-114">[自动承认人员](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)是每个组织者策略，它控制人员是直接加入会议还是在大厅中等待，直到他们被经过身份验证的用户许可。</span><span class="sxs-lookup"><span data-stu-id="19f49-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="19f49-115">[允许匿名用户启动会议](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)是每个组织者策略，它控制匿名人（包括 B2B 和联合用户）是否可以在与会者未经过身份验证的用户的情况下加入用户会议。</span><span class="sxs-lookup"><span data-stu-id="19f49-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="19f49-116">[允许拨入用户绕过会议厅](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)（即将**推出**）是每个组织者策略，它控制通过电话拨入的用户是否直接加入会议或在会议厅中等待，而不管 "是否**自动允许人**" 设置。</span><span class="sxs-lookup"><span data-stu-id="19f49-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="19f49-117">[允许组织者重写前厅浏览设置](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)（**即将推出**）是每个组织者策略，它控制会议组织者是否可以重写用户在计划新会议时**自动**为其设置的前厅浏览设置，并**允许拨入用户绕过会议厅**设置。</span><span class="sxs-lookup"><span data-stu-id="19f49-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="19f49-118">**注意：** 有关 Microsoft 团队会议策略的完整概述，请参阅[在团队中管理会议策略](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)。</span><span class="sxs-lookup"><span data-stu-id="19f49-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
