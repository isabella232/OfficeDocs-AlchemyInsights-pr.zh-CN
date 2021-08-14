---
title: Microsoft 365 组中的欢迎消息
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: 81127b79d4e5a16686ca46d67bfac73c15891938491a702219cd73757c4e106c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53997700"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Microsoft 365 组中的欢迎消息

如果 "UnifiedGroupWelcomeMessageEnabled" 属性为 True，则加入 Microsoft 365 组的新用户将收到欢迎电子邮件。

如果想要禁用欢迎邮件，请使用以下 [LOP-EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) 命令：

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
