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
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059586"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>控制大厅设置和参与Teams

如果要允许所有人（包括拨入用户、外部用户和匿名用户）绕过大厅，请使用 PowerShell 完成此任务。  下面是修改组织的全局会议策略的示例。

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

此 cmdlet 当前需要使用 Skype for Business PowerShell 模块。 若要设置使用此 cmdlet，请查看通过 [PowerShell 管理策略](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)。

设置策略后，需要将策略应用于用户;或者，如果修改了全局策略，该策略将自动应用于用户。 对于任何策略更改，您需要等待至少 **4 小时到 24 小时** ，策略才能生效。 

请务必先查看下面的文档，然后再进行这些更改，以准确了解这允许使用什么。


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>了解Teams控制

这些设置控制哪些会议参与者在获准参加会议之前在会议厅中等待，以及允许他们参加会议的级别。 可以使用 PowerShell 更新尚未在 Teams 管理中心中 ("即将) 会议策略设置。 有关允许所有用户绕过大厅的示例 PowerShell cmdlet，请参阅下文。

- [自动允许人员](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) 是每组织者策略，用于控制用户是直接加入会议，还是等待会议厅，直到经过身份验证的用户允许。

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)允许匿名用户启动会议是按组织者的策略，可控制匿名用户（包括 B2B 和联盟用户）是否可以在未经过身份验证的组织用户的情况下加入用户的会议。

- 允许拨入用户绕过会议厅 [ (即将](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)推出 **)** 是每组织者策略，用于控制通过电话拨入的用户是直接加入会议还是等待在会议厅中，而不考虑"自动允许人员"设置。 

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)允许组织者覆盖即将 (**)** 的大厅设置是一个每组织者策略，可控制会议组织者是否可以覆盖管理员在"自动允许人员"和"允许拨入用户安排新会议时绕过会议厅"中设置的大厅设置。

**注意：** 请参阅 [在会议Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)中管理会议策略，以全面Microsoft Teams会议策略。
