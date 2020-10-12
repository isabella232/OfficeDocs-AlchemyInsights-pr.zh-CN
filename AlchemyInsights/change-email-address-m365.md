---
title: 更改 Microsoft 365 组的电子邮件地址
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48416690"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>更改 Microsoft 365 组的电子邮件地址

可使用管理中心更改 Microsoft 365 组的电子邮件地址。 只需选择组，然后选择 @edit 电子邮件地址。

还可使用以下 EXO PowerShell 命令来更改 Microsoft 365 组的主 SMTP 地址：

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

示例：

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
