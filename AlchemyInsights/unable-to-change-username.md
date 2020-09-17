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
ms.openlocfilehash: 76891b3abe156b736c3bb6da0f6cd1135346dbe2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798654"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="12f6b-102">无法更改用户名</span><span class="sxs-lookup"><span data-stu-id="12f6b-102">Unable to change UserName</span></span>

<span data-ttu-id="12f6b-103">在某些情况下，UPN (UserPrincipalName) 更改不会传播到云。</span><span class="sxs-lookup"><span data-stu-id="12f6b-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="12f6b-104">你可能会在 Office 365 门户中收到验证错误，或者无法更改用户名或电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="12f6b-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="12f6b-105">若要解决此问题，请使用此 PowerShell 命令手动设置 UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="12f6b-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="12f6b-106">**示例：重命名用户**</span><span class="sxs-lookup"><span data-stu-id="12f6b-106">**Example: Rename a user**</span></span>

<span data-ttu-id="12f6b-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="12f6b-107">PowerShellCopy</span></span>

<span data-ttu-id="12f6b-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="12f6b-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="12f6b-109">此命令会将 davidc@contoso.com 重命名为 davidchew@contoso.com。</span><span class="sxs-lookup"><span data-stu-id="12f6b-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="12f6b-110">有关详细信息，请参阅 [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0)。</span><span class="sxs-lookup"><span data-stu-id="12f6b-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>