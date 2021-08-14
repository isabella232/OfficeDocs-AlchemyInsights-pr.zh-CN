---
title: 更改 Microsoft 365 组的电子邮件地址
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
- "4704"
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930719"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>更改 Microsoft 365 组的电子邮件地址

可使用管理中心更改 Microsoft 365 组的电子邮件地址。 只需选择组，然后选择 @edit 电子邮件地址。

你还可以使用以下 LOP-EXO PowerShell 命令来更改 Microsoft 365 组的主 SMTP 地址：

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

示例：

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
