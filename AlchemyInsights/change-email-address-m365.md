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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819070"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>更改 Microsoft 365 组或 Microsoft Teams 的电子邮件地址

可使用 [Microsoft 365 管理中心](https://admin.microsoft.com/) 更改 Microsoft 365 组或 Microsoft Teams 的电子邮件地址。 只需选择组，然后选择 @edit 电子邮件地址。

你还可以使用以下 EXO PowerShell 命令来更改 Microsoft 365 组/Teams 的主 SMTP 地址：

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

示例：

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
