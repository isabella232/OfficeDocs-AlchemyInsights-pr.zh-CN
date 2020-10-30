---
title: 更改强密码要求
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804413"
---
# <a name="change-strong-password-requirement"></a>更改强密码要求

默认情况下，Microsoft 需要强密码。

使用 PowerShell 时，您可以使用以下命令为特定用户禁用强密码：

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

若要对所有用户禁用强密码，请使用：

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [密码策略的详细信息](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [如何使用 PowerShell 连接到 Microsoft 365](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [有关 PowerShell Get-msoluser 命令的详细信息](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
