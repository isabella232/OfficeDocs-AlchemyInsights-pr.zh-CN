---
title: 更改强密码要求
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 21f80a7cc8b00ac56acdb05add1e1bfdfac9d827
ms.sourcegitcommit: c061f1dfa6f557a9ec083dd030b73b121d9864ea
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43286239"
---
# <a name="change-strong-password-requirement"></a>更改强密码要求

默认情况下，Microsoft 需要强密码。 

使用 PowerShell 时，您可以使用此命令为特定用户禁用强密码：<br>
*Get-msoluser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*

- [密码策略的详细信息](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [如何使用 PowerShell 连接到 Office 365](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [有关 PowerShell Get-msoluser 命令的详细信息](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [设置单个用户的密码永不过期](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
