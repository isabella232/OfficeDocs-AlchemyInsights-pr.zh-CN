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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>无法设置主电子邮件地址或更改用户属性

如果为您的环境启用了目录同步, 则无法使用 Microsoft 365 管理中心更改某些用户或对象属性。

若要完全管理同步用户及其所有属性, 请使用本地 active directory 用户和组管理控制台 (adsi .msc)。  

或者, 您可以使用 powershell 更改已同步用户的各个用户或属性, 如以下常见示例中所示: 
- Get-msoluser-UserPrincipalName user@yourdomain.onmicrosoft.com-AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Get-msoluser-UserPrincipalName "user@yourdomain.onmicrosoft.com"-DisplayName "Test User"-LastName "User"-Title "Manager"-部门 "HR"
- Get-msoluser-UserPrincipalName "user@yourdomain.onmicrosoft.com