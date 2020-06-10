---
title: 更改 Microsoft 365 组的电子邮件地址
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
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580647"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>更改 Microsoft 365 组的电子邮件地址

可使用管理中心更改 Microsoft 365 组的电子邮件地址。 只需选择组，然后选择 @edit 电子邮件地址。

你还可以使用以下 LOP-EXO PowerShell 命令来更改 Microsoft 365 组的主 SMTP 地址：

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

示例：

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
