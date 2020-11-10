---
title: 在团队对话中使用 Giphy
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947480"
---
# <a name="using-giphys-in-teams-conversations"></a>在团队对话中使用 Giphy

默认情况下启用团队聊天中的 giphy 访问。 作为管理员，您可以通过 [设置邮件策略](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings)并确保 **在****对话中使用 giphy** 来控制用户是否可以使用 giphy。

如果 Gif 未按预期方式在团队对话中正常工作，请验证：

[邮件策略](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams)需要允许 giphy。 若要使用 PowerShell cmdlet 进行验证，请执行以下操作：

- 验证您是否可以 [使用 PowerShell 管理团队](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)。
- 运行 PowerShell 命令 [CsTeamsMessagingPolicy 全局标识](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) ，并验证 **AllowGiphy** 是否设置为 **TRUE** 。
- 如果 **AllowGiphy** 设置为 **FALSE** ，请运行以下 PowerShell 命令 [集-CsTeamsMessagingPolicy Global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)。

需要启用[可选的连接体验](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences)，以允许访问 Giphy URL。

> [!NOTE]
> 如果为租户配置了多个团队邮件策略，则可以使用 PowerShell 命令 [get-csonlineuser-identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) | 指定分配给受影响的用户的策略的标识。 <user@domain.com> 选择 "TeamsMessagingPolicy"。
