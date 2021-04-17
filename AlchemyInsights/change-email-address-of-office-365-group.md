---
title: 更改 Microsoft 365 组的电子邮件地址
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819034"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="14907-102">更改 Microsoft 365 组的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="14907-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="14907-103">可使用管理中心更改 Microsoft 365 组的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="14907-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="14907-104">只需选择组，然后选择 @edit 电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="14907-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="14907-105">你还可以使用以下 LOP-EXO PowerShell 命令来更改 Microsoft 365 组的主 SMTP 地址：</span><span class="sxs-lookup"><span data-stu-id="14907-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="14907-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="14907-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="14907-107">示例：</span><span class="sxs-lookup"><span data-stu-id="14907-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
