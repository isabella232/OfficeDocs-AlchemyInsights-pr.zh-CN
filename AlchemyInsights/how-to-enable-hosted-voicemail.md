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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055544"
---
# <a name="how-to-enable-hosted-voicemail"></a>如何启用托管语音邮件

若要启用语音邮件， **必须将 HostedVoicemail** 设置为 $true。

使用远程 PowerShell 的用户的 **HostedVoicemail** 属性 (RPS) 。

有关连接到 RPS 的信息，请参阅 Microsoft Teams [PowerShell 概述](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)，详细了解如何连接到 RPS。

1. 管理员Teams登录远程 PowerShell 进行Teams。
1. 在 PowerShell 提示符Teams管理员可运行 **set-csuser user@contoso.com -HostedVoiceMail $true** 其中 sip uri 是问题用户。

> [!NOTE]
> 对策略所做的更改最多可能需要 24 小时才能复制。