---
title: 策略捕获
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
- "3207"
ms.openlocfilehash: 036c171f3c71e60c8c07000b4d0c6ede36bd435c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801653"
---
# <a name="teams-policies"></a>Teams 策略

Microsoft Teams 设置由策略控制。 若要更改，必须配置相应的策略，然后将它应用于用户。 为所有用户执行此操作的最快方法就是修改名为"全局"的默认策略。 

**注意** 策略更改 **_需要至少 4 到 48 小时才能生效_**。 如果创建自定义策略，则需要等待至少 4 小时，然后才能对策略进行其他更改。 然后，可以将该策略应用于用户。 这意味着自定义策略最多可能需要 48 小时才能生效。 全局策略设置为所有用户的默认策略，对全局策略的更改最多可能需要 24 小时才能生效。 如果已创建自定义策略，将策略应用于用户，并且该策略在 48 小时后仍未生效，或者你已修改全局策略并等待至少 24 小时，请打开支持案例。

Teams 策略分为以下几个方面：

- [Teams 策略](https://docs.microsoft.com/MicrosoftTeams/teams-policies) 控制用户在搜索和创建私人频道时发现私人团队。  
- [会议策略](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) 控制用户可以使用 Teams 会议执行哪些操作，包括控制会议厅。 有关大厅问题的帮助，例如配置 Teams 以允许所有人，请参阅控制大厅 [设置和参与级别](https://docs.microsoft.com/alchemyinsights/bypass-lobby)。
- [消息策略](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) 控制用户可以使用聊天和消息执行哪些操作，包括打开或关闭聊天、删除聊天、请求已读回执、使用 giphy 和贴纸等。
- [应用设置](https://docs.microsoft.com/MicrosoftTeams/teams-app-setup-policies) 策略控制哪些应用可供用户使用，包括自定义和第三方应用，以及这些应用的显示顺序。  
- Teams [的数据](https://docs.microsoft.com/microsoftteams/retention-policies) 保留策略位于 Microsoft 365 安全与合规中心。
- Teams 通讯簿策略通过作用域目录 [搜索 进行设置](https://docs.microsoft.com/MicrosoftTeams/teams-scoped-directory-search)。