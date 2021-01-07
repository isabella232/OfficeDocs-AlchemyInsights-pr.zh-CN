---
title: 更改 Microsoft 365 组或 Microsoft Teams 的电子邮件地址
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
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756547"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>更改 Microsoft 365 组或 Microsoft Teams 的电子邮件地址

可使用 [Microsoft 365 管理中心](https://admin.microsoft.com/) 更改 Microsoft 365 组或 Microsoft Teams 的电子邮件地址。 只需选择组，然后选择 @edit 电子邮件地址。

你还可以使用以下 EXO PowerShell 命令来更改 Microsoft 365 组/Teams 的主 SMTP 地址：

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

示例：

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
