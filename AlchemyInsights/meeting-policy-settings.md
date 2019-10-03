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
# <a name="manage-meeting-policies-in-microsoft-teams"></a>在 Microsoft 团队中管理会议策略

会议策略用于控制会议参与者对组织中的用户安排的会议参与者可用的功能。 会议策略的某些功能可能未在团队管理中心中实施（这些功能在文档中被标记为 "即将推出"）。 在这种情况下，或者如果遇到类似 "我们现在无法更新策略，但稍后再试一次" 这一错误（在 Microsoft 团队管理中心，我们建议使用 PowerShell 创建或修改团队会议策略。 

有关会议策略的详细信息，请参阅以下资源：

- 若要了解如何创建策略、进行更改以及将用户分配到策略，请参阅[在团队中管理会议策略](https://docs.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams)。

- 若要使用 PowerShell cmdlet 进行策略更改，请参阅[团队 PowerShell 概述](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)。 
    - 您需要使用[Skype For Business PowerShell 模块](https://www.microsoft.com/download/details.aspx?id=39366)获取团队会议策略。 
    - 有关详细信息，请参阅[*-CsTeamsMeetingPolicy cmdlet 文档](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps)。

**注意：** 可能需要长达24小时才能使策略更改对用户生效。 您可能无法立即对新创建的策略进行更改。等待4小时，并再次尝试修改新创建的策略。 如果仍有问题，请尝试 PowerShell。  