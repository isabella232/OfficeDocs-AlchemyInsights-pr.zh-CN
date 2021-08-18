---
title: 需要将域或电子邮件发件人标记为安全？
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
- "9002921"
- "5673"
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319938"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>需要将域或电子邮件发件人标记为安全？

- **不建议使用安全发件人列表**，因为它会使你的组织容易受到垃圾邮件、网络钓鱼和欺骗攻击。
- 但是，如果有业务需求，我们 **建议** 使用 **[邮件流规则](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**。 我们的指南可确保发件人身份验证（验证发送域是否被欺骗）。 
    **注意**：我们不建议使用安全发件人列表来管理误报，因为垃圾邮件筛选的例外可能会使你的组织容易受到安全攻击。 如果你的用户收到错误标记为垃圾邮件或垃圾电子邮件的邮件，请 **[将邮件和文件报告给 Microsoft](https://protection.office.com/reportsubmission)**。
- **应避免** 使用 Outlook 中的安全发件人、反垃圾邮件策略中允许发件人列表或允许域列表，因为发件人会绕过所有垃圾邮件、欺骗和网络钓鱼保护以及发件人身份验证（SPF、DKIM、DMARC）。此方法最好仅用于临时测试。
- 通过检查“X-Forefront-Antispam-Report”邮件头（SFV：SFE，SFV：SKA，SFV：SKN），可以验证某个电子邮件是否绕过 Antispam 评估，请参阅 **[反垃圾邮件邮件头](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**。
- 由于 Microsoft 希望 [在默认情况下保持客户安全](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)，因此未将某些租户替代应用于恶意软件和高可信度网络钓鱼。 这些替代包括：o   允许发件人列表或允许域列表（反垃圾邮件策略）o   Outlook 安全发件人 O   IP 允许列表（连接筛选） 
- 允许高可信度钓鱼邮件绕过筛选的唯一替代是 Exchange 邮件流规则（也称为传输规则）。 若要使用邮件流规则绕过筛选，请参阅 **[使用邮件流规则来设置邮件中的垃圾邮件可信度级别 (SCL)](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**。