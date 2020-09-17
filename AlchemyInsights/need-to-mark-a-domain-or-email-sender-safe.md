---
title: 需要将域或电子邮件发件人标记为安全？
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
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803235"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>需要将域或电子邮件发件人标记为安全？

- **不建议使用安全发件人列表**，因为它会使你的组织容易受到垃圾邮件、网络钓鱼和欺骗攻击。
- 但是，如果有业务需求，我们**建议**使用**[邮件流规则](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**。 我们的指南可确保发件人身份验证（验证发送域是否被欺骗）。 **注意**：我们不建议使用安全发件人列表来管理误报，因为垃圾邮件筛选的例外可能会使你的组织容易受到安全攻击。 如果你的用户收到错误地标记为垃圾邮件或垃圾电子邮件的邮件，请**[将邮件和文件报告给 Microsoft](https://protection.office.com/reportsubmission)**。
- **应避免**使用 Outlook 中的安全发件人、反垃圾邮件策略中的允许的发件人列表或允许的域列表，因为发件人会绕过所有垃圾邮件、欺骗和网络钓鱼保护以及发件人身份验证（SPF、DKIM、DMARC）。 此方法最好仅用于临时测试。
