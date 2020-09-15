---
title: 旁路前厅浏览
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684940"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>控制团队中的前厅浏览设置和参与级别

如果您想要允许所有人（包括拨入、外部和匿名用户） **绕过会议厅**，请使用 PowerShell 来完成此任务。 下面的示例展示了如何修改组织的全局会议策略。

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

此 cmdlet 当前需要使用 Skype for Business PowerShell 模块。 若要设置为使用此 cmdlet，请 [通过 PowerShell 来查看管理策略](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)。

设置完策略后，需要将其应用于用户;或者，如果您修改了全局策略，它将自动应用于用户。 对于任何策略更改，至少需要等待 **4 小时长达24小时** 才能使策略生效。 

在进行这些更改之前，请务必查看下面的文档，以了解所允许的确切内容。


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>了解团队会议会议厅策略控件

这些设置控制哪些会议参与者在会议厅中等待，并在会议中允许他们参加会议和参与的程度。 您可以使用 PowerShell 更新尚未在团队管理中心中的 "即将到来" ) 实施 (的会议策略设置。 有关允许所有用户绕过会议厅的 PowerShell cmdlet 示例，请参阅下面的示例。

- [自动承认人员](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) 是每个组织者策略，它控制人员是直接加入会议还是在大厅中等待，直到他们被经过身份验证的用户许可。

- [允许匿名用户启动会议](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) 是每个组织者策略，它控制匿名人（包括 B2B 和联合用户）是否可以在与会者未经过身份验证的用户的情况下加入用户会议。

- [允许拨入用户绕过会议厅](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (即将 **推出** 的) 是每个组织者策略，它控制通过电话拨入的用户是否直接加入会议或在会议厅中等待，而不管是否 **自动允许人员** 设置。

- [允许组织者重写前厅浏览设置](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) ** () ** 是每个组织者策略，它控制会议组织者是否可以覆盖管理员设置的前厅浏览设置，管理员可以在计划新会议时将其 **自动授予人员** 并 **允许拨入用户绕过会议厅** 。

**注意：** 有关 Microsoft 团队会议策略的完整概述，请参阅 [在团队中管理会议策略](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) 。
