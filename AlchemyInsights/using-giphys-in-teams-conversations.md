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
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="30edb-102">在团队对话中使用 Giphy</span><span class="sxs-lookup"><span data-stu-id="30edb-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="30edb-103">默认情况下启用团队聊天中的 giphy 访问。</span><span class="sxs-lookup"><span data-stu-id="30edb-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="30edb-104">作为管理员，您可以通过 [设置邮件策略](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings)并确保 **在\*\*\*\*对话中使用 giphy** 来控制用户是否可以使用 giphy。</span><span class="sxs-lookup"><span data-stu-id="30edb-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="30edb-105">如果 Gif 未按预期方式在团队对话中正常工作，请验证：</span><span class="sxs-lookup"><span data-stu-id="30edb-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="30edb-106">[邮件策略](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams)需要允许 giphy。</span><span class="sxs-lookup"><span data-stu-id="30edb-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="30edb-107">若要使用 PowerShell cmdlet 进行验证，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="30edb-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="30edb-108">验证您是否可以 [使用 PowerShell 管理团队](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)。</span><span class="sxs-lookup"><span data-stu-id="30edb-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="30edb-109">运行 PowerShell 命令 [CsTeamsMessagingPolicy 全局标识](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) ，并验证 **AllowGiphy** 是否设置为 **TRUE** 。</span><span class="sxs-lookup"><span data-stu-id="30edb-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="30edb-110">如果 **AllowGiphy** 设置为 **FALSE** ，请运行以下 PowerShell 命令 [集-CsTeamsMessagingPolicy Global-AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)。</span><span class="sxs-lookup"><span data-stu-id="30edb-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="30edb-111">需要启用[可选的连接体验](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences)，以允许访问 Giphy URL。</span><span class="sxs-lookup"><span data-stu-id="30edb-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="30edb-112">如果为租户配置了多个团队邮件策略，则可以使用 PowerShell 命令 [get-csonlineuser-identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) | 指定分配给受影响的用户的策略的标识。 <user@domain.com> 选择 "TeamsMessagingPolicy"。</span><span class="sxs-lookup"><span data-stu-id="30edb-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
