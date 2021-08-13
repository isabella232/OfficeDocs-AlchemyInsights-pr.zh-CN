---
title: 更改 Microsoft 365 组或 Microsoft Teams 的电子邮件地址
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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995612"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>更改 Microsoft 365 组或 Microsoft Teams 的电子邮件地址

可使用 [Microsoft 365 管理中心](https://admin.microsoft.com/)更改 Microsoft 365 组或 Microsoft Teams 的电子邮件地址。只需选择相应组，然后选择 @edit 电子邮件地址。

你还可以使用以下 EXO PowerShell 命令来更改 Microsoft 365 组/Teams 的主 SMTP 地址：

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

示例：

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
