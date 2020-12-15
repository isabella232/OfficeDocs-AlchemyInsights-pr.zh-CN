---
title: 更改 Microsoft 365 组的电子邮件地址
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: f54ca5df09d0604f6d58c6c8a41dc907485e1f04
ms.sourcegitcommit: beb9715ac0c8e8333fef6764ecd346b7401a2612
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/10/2020
ms.locfileid: "48416690"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="aadea-102">更改 Microsoft 365 组的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="aadea-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="aadea-103">可使用管理中心更改 Microsoft 365 组的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="aadea-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="aadea-104">只需选择组，然后选择 @edit 电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="aadea-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="aadea-105">你还可以使用以下 LOP-EXO PowerShell 命令来更改 Microsoft 365 组的主 SMTP 地址：</span><span class="sxs-lookup"><span data-stu-id="aadea-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

<span data-ttu-id="aadea-106">示例：</span><span class="sxs-lookup"><span data-stu-id="aadea-106">Example:</span></span>

`et-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
