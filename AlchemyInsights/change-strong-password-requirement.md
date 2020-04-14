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
# <a name="change-strong-password-requirement"></a><span data-ttu-id="f46af-102">更改强密码要求</span><span class="sxs-lookup"><span data-stu-id="f46af-102">Change strong password requirement</span></span>

<span data-ttu-id="f46af-103">默认情况下，Microsoft 需要强密码。</span><span class="sxs-lookup"><span data-stu-id="f46af-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="f46af-104">使用 PowerShell 时，您可以使用此命令为特定用户禁用强密码：</span><span class="sxs-lookup"><span data-stu-id="f46af-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="f46af-105">*Get-msoluser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="f46af-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="f46af-106">密码策略的详细信息</span><span class="sxs-lookup"><span data-stu-id="f46af-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="f46af-107">如何使用 PowerShell 连接到 Office 365</span><span class="sxs-lookup"><span data-stu-id="f46af-107">How to connect to Office 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="f46af-108">有关 PowerShell Get-msoluser 命令的详细信息</span><span class="sxs-lookup"><span data-stu-id="f46af-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
- [<span data-ttu-id="f46af-109">设置单个用户的密码永不过期</span><span class="sxs-lookup"><span data-stu-id="f46af-109">Set an individual user's password to never expire</span></span>](https://docs.microsoft.com/microsoft-365/admin/add-users/set-password-to-never-expire)
