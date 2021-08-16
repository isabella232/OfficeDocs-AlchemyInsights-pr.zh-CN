---
title: 无法更改用户名
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 3088a7b939e7b88319ff688ea94fa71d7fa540787cde31cfd864551113caf149
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020218"
---
# <a name="unable-to-change-username"></a>无法更改用户名

在某些情况下，UPN (UserPrincipalName) 更改不会传播到云。 你可能会在 Office 365 门户中收到验证错误，或者无法更改用户名或电子邮件地址。 若要解决此问题，请使用此 PowerShell 命令手动设置 UserPrincipalName。

**示例：重命名用户**

PowerShellCopy

PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"

此命令会将 davidc@contoso.com 重命名为 davidchew@contoso.com。

有关详细信息，请参阅 [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0)。