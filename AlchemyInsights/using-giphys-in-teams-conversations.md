---
title: 在对话中Teams Giphys
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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104298"
---
# <a name="using-giphys-in-teams-conversations"></a>在对话中Teams Giphys

默认情况下，启用Teams聊天中的 Giphys 访问。 作为管理员，您可以通过设置消息策略并确保在对话中使用 Giphys [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings)为 On 来控制 **Giphys** 是否 **可供用户使用**。

如果 GIF 在对话中未Teams，请验证：

邮件 [策略需要](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) 允许 Giphys。 若要使用 PowerShell cmdlet 进行验证，请运行：

- 验证您是否可以使用[PowerShell Teams管理服务](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)。
- 运行 PowerShell 命令 [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) 并验证 **AllowGiphy** 是否设置为 **TRUE**。
- 如果 **AllowGiphy** 设置为 **FALSE，** 请运行以下 PowerShell 命令 [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True。](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[需要启用](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) 可选连接体验以允许访问 Giphy URL。

> [!NOTE]
> 如果为租户配置了多个 Teams 邮件策略，可以使用 PowerShell 命令[Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) | <user@domain.com>选择 TeamsMessagingPolicy。
