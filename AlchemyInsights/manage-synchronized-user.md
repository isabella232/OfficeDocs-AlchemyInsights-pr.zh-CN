---
title: 管理同步用户
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541972"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="d2fd5-102">无法设置主电子邮件地址或更改用户属性</span><span class="sxs-lookup"><span data-stu-id="d2fd5-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="d2fd5-103">如果为您的环境启用了目录同步, 则无法使用 Microsoft 365 管理中心更改某些用户或对象属性。</span><span class="sxs-lookup"><span data-stu-id="d2fd5-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="d2fd5-104">若要完全管理同步用户及其所有属性, 请使用本地 active directory 用户和组管理控制台 (adsi .msc)。</span><span class="sxs-lookup"><span data-stu-id="d2fd5-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="d2fd5-105">或者, 您可以使用 powershell 更改已同步用户的各个用户或属性, 如以下常见示例中所示:</span><span class="sxs-lookup"><span data-stu-id="d2fd5-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="d2fd5-106">Get-msoluser-UserPrincipalName user@yourdomain.onmicrosoft.com-AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="d2fd5-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="d2fd5-107">Get-msoluser-UserPrincipalName "user@yourdomain.onmicrosoft.com"-DisplayName "Test User"-LastName "User"-Title "Manager"-部门 "HR"</span><span class="sxs-lookup"><span data-stu-id="d2fd5-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="d2fd5-108">Get-msoluser-UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="d2fd5-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>