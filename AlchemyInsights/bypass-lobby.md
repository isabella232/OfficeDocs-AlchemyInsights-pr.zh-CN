---
title: 绕过大厅
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820024"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>控制大厅设置和参与 Teams 的级别

如果要允许所有人（包括拨入用户、外部用户和匿名用户）绕过大厅，请使用 PowerShell 完成此任务。  下面是修改组织的全局会议策略的示例。

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

此 cmdlet 当前需要使用 Skype for Business PowerShell 模块。 若要设置使用此 cmdlet，请查看通过 [PowerShell 管理策略](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)。

设置策略后，需要将策略应用于用户;或者，如果修改了全局策略，该策略将自动应用于用户。 对于任何策略更改，您需要等待至少 **4 小时到 24 小时** ，策略才能生效。 

请务必先查看下面的文档，然后再进行这些更改，以准确了解这允许使用什么。


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>了解 Teams 会议厅策略控制

这些设置控制哪些会议参与者在获准参加会议之前在会议厅中等待，以及允许他们参加会议的级别。 可以使用 PowerShell 更新尚未实现的会议策略设置， (Teams 管理中心中标记为"即将) "的会议策略设置。 有关允许所有用户绕过大厅的示例 PowerShell cmdlet，请参阅下文。

- [自动允许人员](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) 是每组织者策略，用于控制用户是直接加入会议，还是等待会议厅，直到经过身份验证的用户允许。

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)允许匿名用户启动会议是按组织者的策略，可控制匿名用户（包括 B2B 和联盟用户）是否可以在未经过身份验证的组织用户的情况下加入用户的会议。

- 允许拨入用户绕过会议厅 [ (即将](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)推出 **)** 是每组织者策略，用于控制通过电话拨入的用户是直接加入会议还是等待在会议厅中，而不考虑"自动允许人员"设置。 

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)允许组织者覆盖即将 (**)** 的大厅设置是一个每组织者策略，可控制会议组织者是否可以覆盖管理员在"自动允许人员"和"允许拨入用户安排新会议时绕过会议厅"中设置的大厅设置。

**注意：** 有关 Microsoft Teams [会议策略](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) 的完整概述，请参阅在 Teams 中管理会议策略。
