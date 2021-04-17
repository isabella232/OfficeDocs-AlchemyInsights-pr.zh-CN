---
title: 会议策略设置
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825433"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>在 Microsoft Teams 中管理会议策略

**注意：策略更改最多可能需要 24 小时才能对用户生效。** 可能无法立即对新创建的策略进行更改;等待 4 小时，然后再次尝试修改新创建的策略。

会议策略用于控制可供组织中用户安排的会议的会议参与者使用的功能。 会议策略的一些功能可能尚未在 Teams 管理中心中实现 (文档"即将推出"这些) 。 在这种情况下，或者如果你在 Microsoft Teams 管理中心收到类似"我们现在无法更新策略，但稍后重试"的错误，我们建议你使用 PowerShell 创建或修改 Teams 会议策略。 

有关会议策略详细信息，请参阅以下资源：

- 若要了解如何创建策略、进行更改以及向策略分配用户，请参阅在 Teams 中 [管理会议策略](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)。

- 若要使用 PowerShell cmdlet 更改策略，请参阅 [Teams PowerShell 概述](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)。 
    - 你需要将 Skype [for Business PowerShell 模块用于](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) Teams 会议策略。 
    - 有关详细信息 [，请参阅 *-CsTeamsMeetingPolicy cmdlet](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) 文档。

