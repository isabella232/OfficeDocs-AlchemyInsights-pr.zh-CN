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
# <a name="control-lobby-settings-and-level-of-participation"></a>控制前厅浏览设置和参与级别

这些设置控制哪些会议参与者在会议厅中等待，并在会议中允许他们参加会议和参与的程度。 您可以使用 Powershell 更新团队管理中心中尚未实现的会议策略设置（标为 "即将推出"）。  有关允许所有用户绕过会议厅的 PowerShell cmdlet 示例，请参阅下面的示例。  

- [自动承认人员](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people)是每个组织者策略，它控制人员是直接加入会议还是在大厅中等待，直到他们被经过身份验证的用户许可。

- [允许匿名用户启动会议](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting)是每个组织者策略，它控制匿名人（包括 B2B 和联合用户）是否可以在与会者未经过身份验证的用户的情况下加入用户会议。

- [允许拨入用户绕过会议厅](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon)（即将**推出**）是每个组织者策略，它控制通过电话拨入的用户是否直接加入会议或在会议厅中等待，而不管 "是否**自动允许人**" 设置。

- [允许组织者重写前厅浏览设置](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon)（即将**推出**）是每个组织者策略，它控制会议组织者是否可以覆盖管理员设置的前厅浏览设置，以**自动承认人员**并**允许拨入用户**在安排新会议时绕过会议厅。

**注意：** 有关 Microsoft 团队会议策略的完整概述，请参阅[在团队中管理会议策略](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)。 


**PowerShell 示例**

如果您希望允许所有人（包括外部或匿名用户）绕过会议厅，您还可以使用 PowerShell 来完成此任务。  下面的示例展示了如何修改组织的全局会议策略。   

（请务必先查看上面的文档，然后再进行这些更改，以了解此功能的具体内容。）

CsTeamsMeetingPolicy-Identity Global-AutoAdmittedUsers "Everyone"-AllowPSTNUsersToBypassLobby $True

有关详细信息，请参阅[CsTeamsMeetingPolicy](https://docs.microsoft.com/powershell/module/skype/set-csteamsmeetingpolicy?view=skype-ps)。
