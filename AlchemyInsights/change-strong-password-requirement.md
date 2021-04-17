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
# <a name="change-strong-password-requirement"></a><span data-ttu-id="a63fd-102">更改强密码要求</span><span class="sxs-lookup"><span data-stu-id="a63fd-102">Change strong password requirement</span></span>

<span data-ttu-id="a63fd-103">默认情况下，Microsoft 需要强密码。</span><span class="sxs-lookup"><span data-stu-id="a63fd-103">Microsoft requires strong passwords by default.</span></span>

<span data-ttu-id="a63fd-104">使用 PowerShell，可以使用以下命令为特定用户禁用强密码：</span><span class="sxs-lookup"><span data-stu-id="a63fd-104">Using PowerShell, you can disable strong passwords for specific users with these commands:</span></span>

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

<span data-ttu-id="a63fd-105">若要禁用所有用户的强密码，请使用：</span><span class="sxs-lookup"><span data-stu-id="a63fd-105">To disable strong passwords for all users, use:</span></span>

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [<span data-ttu-id="a63fd-106">有关密码策略详细信息</span><span class="sxs-lookup"><span data-stu-id="a63fd-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="a63fd-107">如何使用 PowerShell 连接到 Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a63fd-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="a63fd-108">有关 PowerShell MsolUser 命令详细信息</span><span class="sxs-lookup"><span data-stu-id="a63fd-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
