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
ms.openlocfilehash: a2605bcd66f61de811ebb6e273e4ef1cff2b0119
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47733677"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>更改 Microsoft 365 组的电子邮件地址

可使用管理中心更改 Microsoft 365 组的电子邮件地址。 只需选择组，然后选择 @edit 电子邮件地址。

你还可以使用以下 LOP-EXO PowerShell 命令来更改 Microsoft 365 组的主 SMTP 地址：

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

示例：

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
