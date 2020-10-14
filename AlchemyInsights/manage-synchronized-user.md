---
title: 管理同步用户
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
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451390"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="64532-102">无法设置主电子邮件地址、更改用户属性或删除/删除同步用户</span><span class="sxs-lookup"><span data-stu-id="64532-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="64532-103">如果为您的环境启用了目录同步，则无法使用 Microsoft 365 管理中心更改某些用户或对象属性。</span><span class="sxs-lookup"><span data-stu-id="64532-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="64532-104">若要完全管理同步用户及其所有属性，请使用本地 active directory 用户和组管理控制台 (adsiedit) 。</span><span class="sxs-lookup"><span data-stu-id="64532-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="64532-105">或者，您可以使用 powershell 更改已同步用户的各个用户或属性，如以下常见示例中所示：</span><span class="sxs-lookup"><span data-stu-id="64532-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span>

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
