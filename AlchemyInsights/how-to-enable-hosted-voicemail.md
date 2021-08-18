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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318638"
---
# <a name="how-to-enable-hosted-voicemail"></a>如何启用托管语音邮件

若要启用语音邮件， **必须将 HostedVoicemail** 设置为 $true。

使用远程 PowerShell 的用户的 **HostedVoicemail** 属性 (RPS) 。

有关连接到 RPS 的信息，请参阅 Microsoft Teams [PowerShell 概述](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)，详细了解如何连接到 RPS。

1. 管理员Teams登录远程 PowerShell 进行Teams。
1. 在 PowerShell 提示Teams管理员可运行 **set-csuser user@contoso.com -HostedVoiceMail $true** 其中 sip uri 是问题用户。

**注意**：对策略所做的更改最多可能需要 24 小时才能复制。