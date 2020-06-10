---
title: 更改 Microsoft 365 组的电子邮件地址
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580647"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a><span data-ttu-id="f3da2-102">更改 Microsoft 365 组的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="f3da2-102">Change email address of a Microsoft 365 group</span></span>

<span data-ttu-id="f3da2-103">可使用管理中心更改 Microsoft 365 组的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="f3da2-103">You can change the email address of a Microsoft 365 group by using the admin center.</span></span> <span data-ttu-id="f3da2-104">只需选择组，然后选择 @edit 电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="f3da2-104">Just select the group and select @edit email address.</span></span>

<span data-ttu-id="f3da2-105">你还可以使用以下 LOP-EXO PowerShell 命令来更改 Microsoft 365 组的主 SMTP 地址：</span><span class="sxs-lookup"><span data-stu-id="f3da2-105">You can also use following the EXO PowerShell command to change the primary SMTP address of a Microsoft 365 group:</span></span>

<span data-ttu-id="f3da2-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span><span class="sxs-lookup"><span data-stu-id="f3da2-106">Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address></span></span>

<span data-ttu-id="f3da2-107">示例：</span><span class="sxs-lookup"><span data-stu-id="f3da2-107">Example:</span></span>

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
