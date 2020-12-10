---
title: 如何启用托管语音邮件
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608820"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="7aeb9-102">如何启用托管语音邮件</span><span class="sxs-lookup"><span data-stu-id="7aeb9-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="7aeb9-103">若要启用语音邮件， **HostedVoicemail** 必须设置为 $true。</span><span class="sxs-lookup"><span data-stu-id="7aeb9-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="7aeb9-104">使用远程 PowerShell (RPS) 的用户的 **HostedVoicemail** 属性。</span><span class="sxs-lookup"><span data-stu-id="7aeb9-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="7aeb9-105">有关连接到 RPS 的详细信息，请参阅 [Microsoft 团队 PowerShell 概述](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) ，了解有关连接 rps 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="7aeb9-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="7aeb9-106">团队管理员应登录到适用于团队的远程 PowerShell。</span><span class="sxs-lookup"><span data-stu-id="7aeb9-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="7aeb9-107">从 PowerShell 提示符中，团队管理员可以运行 **get-csuser user@contoso.com-HostedVoiceMail $true** ，其中 sip uri 是有问题的用户。</span><span class="sxs-lookup"><span data-stu-id="7aeb9-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="7aeb9-108">对策略所做的更改可能需要长达24小时才能进行复制。</span><span class="sxs-lookup"><span data-stu-id="7aeb9-108">Changes to policies can take up to 24 hours to replicate.</span></span>