---
title: 创建共享邮箱时发生代理地址错误
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: 7c15d5db5445fbe4c3ec22878f180f48d2da4f90369f2e6f223916646eb19c12
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54062898"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>创建邮箱或其他启用电子邮件的对象时发生代理地址错误

如果您尝试创建启用电子邮件的对象 (邮箱、共享邮箱等 ) 并且收到错误"代理地址"SMTP:alias@domain.com"已在使用..."，则您选择的电子邮件地址已由组织中另一个启用电子邮件的对象使用。
  
您需要查找具有此电子邮件地址的用户、组、共享邮箱或公用文件夹，并将其删除或更改其电子邮件地址。 然后，可以使用释放的电子邮件地址创建新的启用电子邮件的对象。 使用主页上的搜索来查找它。 您还可以使用以下 PowerShell Exchange Online搜索它：

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
如果不想删除现有电子邮件地址，请为要创建的新对象选择一个新电子邮件地址。
  