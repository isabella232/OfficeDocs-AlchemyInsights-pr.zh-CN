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
ms.openlocfilehash: bf8be9ffe2bfa45ed2cf149c1c4fa118b40e816d
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "37768430"
---
# <a name="control-lobby-settings-and-level-of-participation"></a>控制前厅浏览设置和参与级别

如果您希望允许所有人（包括拨入、外部和匿名用户）绕过 Microsoft 团队中的大厅，则可以使用 PowerShell 执行此操作。 下面的示例展示了如何修改组织的全局会议策略：

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

此 cmdlet 当前需要使用 Skype for Business PowerShell 模块。 若要获取安装程序以使用此 cmdlet，请[通过 PowerShell 查看管理策略](https://docs.microsoft.com/en-us/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)。

您可以设置新策略，然后需要将其应用于用户。 如果您修改全局策略，它将自动应用于用户。 对于任何策略更改，至少需要等待4小时，且最长为24小时才能使策略生效。

在进行这些更改之前，请务必查看下面的文档，以了解所允许的确切内容。

## <a name="understanding-teams-meeting-lobby-policy-controls"></a>了解团队会议会议厅策略控件

- [自动承认人员](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)是每个组织者策略，它控制人员是直接加入会议还是在大厅中等待，直到他们被经过身份验证的用户许可。

- [允许匿名用户启动会议](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)是每个组织者策略，它控制匿名人（包括 B2B 和联合用户）是否可以在与会者未经过身份验证的用户的情况下加入用户会议。

- [允许拨入用户绕过会议厅](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)（即将**推出**）是每个组织者策略，它控制通过电话拨入的用户是否直接加入会议或在会议厅中等待，而不管 "是否**自动允许人**" 设置。

- [允许组织者重写前厅浏览设置](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)（**即将推出**）是每个组织者策略，它控制会议组织者是否可以重写用户在计划新会议时**自动**为其设置的前厅浏览设置，并**允许拨入用户绕过会议厅**设置。

**注意：** 有关 Microsoft 团队会议策略的完整概述，请参阅[在团队中管理会议策略](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)。
