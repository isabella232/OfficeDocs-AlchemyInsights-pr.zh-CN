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
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792122"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="581bb-102">需要将域或电子邮件发件人标记为安全？</span><span class="sxs-lookup"><span data-stu-id="581bb-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="581bb-103">**不建议使用安全发件人列表**，因为它会使你的组织容易受到垃圾邮件、网络钓鱼和欺骗攻击。</span><span class="sxs-lookup"><span data-stu-id="581bb-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="581bb-104">但是，如果有业务需求，我们 **建议** 使用 **[邮件流规则](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**。</span><span class="sxs-lookup"><span data-stu-id="581bb-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="581bb-105">我们的指南可确保发件人身份验证（验证发送域是否被欺骗）。</span><span class="sxs-lookup"><span data-stu-id="581bb-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="581bb-106">**注意**：我们不建议使用安全发件人列表来管理误报，因为垃圾邮件筛选的例外可能会使你的组织容易受到安全攻击。</span><span class="sxs-lookup"><span data-stu-id="581bb-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="581bb-107">如果你的用户收到错误地标记为垃圾邮件或垃圾电子邮件的邮件，请 **[将邮件和文件报告给 Microsoft](https://protection.office.com/reportsubmission)**。</span><span class="sxs-lookup"><span data-stu-id="581bb-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="581bb-108">**应避免** 使用 Outlook 中的安全发件人、反垃圾邮件策略中的允许的发件人列表或允许的域列表，因为发件人会绕过所有垃圾邮件、欺骗和网络钓鱼保护以及发件人身份验证（SPF、DKIM、DMARC）。</span><span class="sxs-lookup"><span data-stu-id="581bb-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="581bb-109">此方法最好仅用于临时测试。</span><span class="sxs-lookup"><span data-stu-id="581bb-109">This method is best used for temporary testing only.</span></span>
