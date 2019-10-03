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
ms.openlocfilehash: de665ca6defcd0d00d227435473e5a4ccf61bc82
ms.sourcegitcommit: 0495112ad4fd0e695140ec66d190e62f03030584
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37376537"
---
# <a name="control-lobby-settings-and-level-of-participation"></a><span data-ttu-id="2da61-102">控制前厅浏览设置和参与级别</span><span class="sxs-lookup"><span data-stu-id="2da61-102">Control lobby settings and level of participation</span></span>

<span data-ttu-id="2da61-103">这些设置控制哪些会议参与者在会议厅中等待，并在会议中允许他们参加会议和参与的程度。</span><span class="sxs-lookup"><span data-stu-id="2da61-103">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="2da61-104">您可以使用 Powershell 更新团队管理中心中尚未实现的会议策略设置（标为 "即将推出"）。</span><span class="sxs-lookup"><span data-stu-id="2da61-104">You can use Powershell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span>  <span data-ttu-id="2da61-105">有关允许所有用户绕过会议厅的 PowerShell cmdlet 示例，请参阅下面的示例。</span><span class="sxs-lookup"><span data-stu-id="2da61-105">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>  

- <span data-ttu-id="2da61-106">[自动承认人员](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)是每个组织者策略，它控制人员是直接加入会议还是在大厅中等待，直到他们被经过身份验证的用户许可。</span><span class="sxs-lookup"><span data-stu-id="2da61-106">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="2da61-107">[允许匿名用户启动会议](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)是每个组织者策略，它控制匿名人（包括 B2B 和联合用户）是否可以在与会者未经过身份验证的用户的情况下加入用户会议。</span><span class="sxs-lookup"><span data-stu-id="2da61-107">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="2da61-108">[允许拨入用户绕过会议厅](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)（即将**推出**）是每个组织者策略，它控制通过电话拨入的用户是否直接加入会议或在会议厅中等待，而不管 "是否**自动允许人**" 设置。</span><span class="sxs-lookup"><span data-stu-id="2da61-108">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="2da61-109">[允许组织者重写前厅浏览设置](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)（即将**推出**）是每个组织者策略，它控制会议组织者是否可以覆盖管理员设置的前厅浏览设置，以**自动承认人员**并**允许拨入用户**在安排新会议时绕过会议厅。</span><span class="sxs-lookup"><span data-stu-id="2da61-109">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="2da61-110">**注意：** 有关 Microsoft 团队会议策略的完整概述，请参阅[在团队中管理会议策略](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)。</span><span class="sxs-lookup"><span data-stu-id="2da61-110">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span> 


<span data-ttu-id="2da61-111">**PowerShell 示例**</span><span class="sxs-lookup"><span data-stu-id="2da61-111">**PowerShell example**</span></span>

<span data-ttu-id="2da61-112">如果您希望允许所有人（包括外部或匿名用户）绕过会议厅，您还可以使用 PowerShell 来完成此任务。</span><span class="sxs-lookup"><span data-stu-id="2da61-112">If you'd like to allow everyone, including external or anonymous users, to bypass the lobby, you can also use PowerShell to accomplish this task.</span></span>  <span data-ttu-id="2da61-113">下面的示例展示了如何修改组织的全局会议策略。</span><span class="sxs-lookup"><span data-stu-id="2da61-113">Here's an example of modifying the global meeting policy for your organization.</span></span>   

<span data-ttu-id="2da61-114">（请务必先查看上面的文档，然后再进行这些更改，以了解此功能的具体内容。）</span><span class="sxs-lookup"><span data-stu-id="2da61-114">(Be sure to review the documentation above before making these changes to understand exactly what this allows.)</span></span>

<span data-ttu-id="2da61-115">CsTeamsMeetingPolicy-Identity Global-AutoAdmittedUsers "Everyone"-AllowPSTNUsersToBypassLobby $True</span><span class="sxs-lookup"><span data-stu-id="2da61-115">Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True</span></span>

<span data-ttu-id="2da61-116">有关详细信息，请参阅[CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps)。</span><span class="sxs-lookup"><span data-stu-id="2da61-116">For more information, see [Set-CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps).</span></span>
