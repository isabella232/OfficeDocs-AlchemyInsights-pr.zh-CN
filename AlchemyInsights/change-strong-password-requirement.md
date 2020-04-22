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
ms.openlocfilehash: a054735a0c139c90d76098297bb9984d37464d3b
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706551"
---
# <a name="change-strong-password-requirement"></a><span data-ttu-id="ac168-102">更改强密码要求</span><span class="sxs-lookup"><span data-stu-id="ac168-102">Change strong password requirement</span></span>

<span data-ttu-id="ac168-103">默认情况下，Microsoft 需要强密码。</span><span class="sxs-lookup"><span data-stu-id="ac168-103">Microsoft requires strong passwords by default.</span></span> 

<span data-ttu-id="ac168-104">使用 PowerShell 时，您可以使用此命令为特定用户禁用强密码：</span><span class="sxs-lookup"><span data-stu-id="ac168-104">Using PowerShell, you can disable strong passwords for specific users with this command:</span></span><br>
<span data-ttu-id="ac168-105">*Get-msoluser – UserPrincipalName <UserPrincipalName> – StrongPasswordRequired $false*</span><span class="sxs-lookup"><span data-stu-id="ac168-105">*Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false*</span></span>

- [<span data-ttu-id="ac168-106">密码策略的详细信息</span><span class="sxs-lookup"><span data-stu-id="ac168-106">More information on password policy</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [<span data-ttu-id="ac168-107">如何使用 PowerShell 连接到 Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ac168-107">How to connect to Microsoft 365 with PowerShell</span></span>](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [<span data-ttu-id="ac168-108">有关 PowerShell Get-msoluser 命令的详细信息</span><span class="sxs-lookup"><span data-stu-id="ac168-108">More information on PowerShell MsolUser commands</span></span>](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
