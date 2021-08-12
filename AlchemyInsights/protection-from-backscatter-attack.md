---
title: 防止退信式垃圾邮件攻击
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8c6b1cfe79d322702279877ff351397a366fa246710c04e25181a675ad2fdeab
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911220"
---
# <a name="protection-from-backscatter-attack"></a>防止退信式垃圾邮件攻击

退信式垃圾邮件是针对你未发送的邮件收到的未送达报告（也称为 NDR 或退回邮件）。 垃圾邮件发送者伪造（欺骗）邮件的 **发件人：** 地址，并且他们经常使用真实的电子邮件地址来增强邮件的信誉。 因此，当垃圾邮件发送者不可避免地将邮件发送给不存在的收件人时，实际上会诱使目标电子邮件服务器将 NDR 中无法送达的邮件退回给 **发件人：** 地址的伪造发件人。

有关其他信息，请参阅 [EOP 中的退信式垃圾邮件](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)。

**启用退信式垃圾邮件保护**

若要启用退信式垃圾邮件保护，请按照以下路径操作。

**protection.office.com >“威胁管理”>“策略”>“反垃圾邮件”>“选择垃圾邮件筛选策略并编辑策略”>“垃圾邮件属性”>“标记为垃圾邮件”>“NDR 退信式垃圾邮件”> 将其设置为“开”**

如果你认为帐户已被盗用，请参阅以下内容：

- [响应被盗用的电子邮件帐户](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [在 Office 365 中从“受限的用户”门户中删除被阻止的用户](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



