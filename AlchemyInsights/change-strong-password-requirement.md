---
title: 更改强密码要求
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 53affd2a347c004e7b21b353c2b3df98bc30a585
ms.sourcegitcommit: a7e5ca472000dfec471950bafd12eee8d7144f74
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35701574"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="21581-102">更改强密码要求</span><span class="sxs-lookup"><span data-stu-id="21581-102">Change strong password requirement</span></span>

<span data-ttu-id="21581-103">默认情况下需要强密码。</span><span class="sxs-lookup"><span data-stu-id="21581-103">Strong passwords are required by default.</span></span> 

<span data-ttu-id="21581-104">使用 PowerShell 您可以使用此命令为特定用户禁用强密码:</span><span class="sxs-lookup"><span data-stu-id="21581-104">Using PowerShell you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="21581-105">*Get-msoluser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="21581-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="21581-106">密码策略的详细信息</span><span class="sxs-lookup"><span data-stu-id="21581-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="21581-107">如何使用 PowerShell 连接到 O365</span><span class="sxs-lookup"><span data-stu-id="21581-107">How to connect to O365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="21581-108">有关 PowerShell Get-msoluser 命令的详细信息</span><span class="sxs-lookup"><span data-stu-id="21581-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)