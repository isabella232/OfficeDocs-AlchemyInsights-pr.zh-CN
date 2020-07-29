---
title: 多个对象的电子邮件地址与标识相同
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431341"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>多个对象的电子邮件地址与标识相同

**多个对象**

发生此错误的常见原因之一是，如果有多个对象的电子邮件地址与标识相同，则无法正确路由 Outlook Web Access 请求。 若要查找这些对象，请运行以下命令：

· Get-Recipient <email address>

· Get-User <email address>

· Get-User <email address> -SoftDeletedUser

· Get-Contact <email address>

· Get-Mailbox <email address> -PublicFolder

· Get-Mailbox <email address> -IncludeSoftDeletedMailbox

· Get-Mailbox <email address> -InactiveMailboxOnly

若要解决该问题，请删除具有相同电子邮件标识的多个对象，并确保有一个对象具有特定电子邮件标识，并且其收件人类型为 UserMailbox。

**相同地址用于企业和使用者邮箱**

另一种原因是将相同地址用于企业和使用者邮箱。 在这种情况下，用户必须更改其主要的使用者别名，直至 Cafe 支持此方案。 这是一个永久性错误，没有干预就不会消失。

有关详细信息，请参阅[更改 Microsoft 帐户的电子邮件地址或电话号码](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account)。