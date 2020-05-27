---
title: Microsoft 365 组中的欢迎消息
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44320445"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Microsoft 365 组中的欢迎消息

如果 "UnifiedGroupWelcomeMessageEnabled" 属性为 True，则加入 Microsoft 365 组的新用户将收到欢迎电子邮件。

如果想要禁用欢迎邮件，请使用以下 [LOP-EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) 命令：

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
