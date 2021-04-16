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
ms.openlocfilehash: 6c46ba1b2c2c94e21d7c76e45df1d416ba423faf
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806396"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Microsoft 365 组中的欢迎消息

如果 "UnifiedGroupWelcomeMessageEnabled" 属性为 True，则加入 Microsoft 365 组的新用户将收到欢迎电子邮件。

如果想要禁用欢迎邮件，请使用以下 [LOP-EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) 命令：

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
