---
title: 更改强密码要求
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818458"
---
# <a name="change-strong-password-requirement"></a>更改强密码要求

默认情况下，Microsoft 需要强密码。

使用 PowerShell，可以使用以下命令为特定用户禁用强密码：

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

若要禁用所有用户的强密码，请使用：

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [有关密码策略详细信息](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [如何使用 PowerShell 连接到 Microsoft 365](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [有关 PowerShell MsolUser 命令详细信息](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
