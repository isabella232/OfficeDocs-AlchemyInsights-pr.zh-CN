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
ms.openlocfilehash: 57d1e2d696a8be42b5f868f021d829bf019349bf
ms.sourcegitcommit: 3994cece80410371330b39f7b79b1b1c1bfcf648
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/08/2021
ms.locfileid: "52286670"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="3b580-102">需要将域或电子邮件发件人标记为安全？</span><span class="sxs-lookup"><span data-stu-id="3b580-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="3b580-103">**不建议使用安全发件人列表**，因为它会使你的组织容易受到垃圾邮件、网络钓鱼和欺骗攻击。</span><span class="sxs-lookup"><span data-stu-id="3b580-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="3b580-104">但是，如果有业务需求，我们 **建议** 使用 **[邮件流规则](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**。</span><span class="sxs-lookup"><span data-stu-id="3b580-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="3b580-105">我们的指南可确保发件人身份验证（验证发送域是否被欺骗）。</span><span class="sxs-lookup"><span data-stu-id="3b580-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="3b580-106">**注意**：我们不建议使用安全发件人列表来管理误报，因为垃圾邮件筛选的例外可能会使你的组织容易受到安全攻击。</span><span class="sxs-lookup"><span data-stu-id="3b580-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="3b580-107">如果你的用户收到错误地标记为垃圾邮件或垃圾电子邮件的邮件，请 **[将邮件和文件报告给 Microsoft](https://protection.office.com/reportsubmission)**。</span><span class="sxs-lookup"><span data-stu-id="3b580-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="3b580-p102">**应避免** 使用 Outlook 中的安全发件人、反垃圾邮件策略中允许发件人列表或允许域列表，因为发件人会绕过所有垃圾邮件、欺骗和网络钓鱼保护以及发件人身份验证（SPF、DKIM、DMARC）。此方法最好仅用于临时测试。</span><span class="sxs-lookup"><span data-stu-id="3b580-p102">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC). This method is best used for temporary testing only.</span></span>
- <span data-ttu-id="3b580-110">通过检查“X-Forefront-Antispam-Report”邮件头（SFV：SFE，SFV：SKA，SFV：SKN），可以验证某个电子邮件是否绕过 Antispam 评估，请参阅 **[反垃圾邮件邮件头](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**。</span><span class="sxs-lookup"><span data-stu-id="3b580-110">The validation that a certain email bypassed Antispam evaluation can be done by checking “X-Forefront-Antispam-Report" message header (SFV:SFE, SFV:SKA, SFV:SKN), see **[Anti-spam message headers](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**.</span></span>
- <span data-ttu-id="3b580-111">由于 Microsoft 希望 [在默认情况下保持客户安全](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)，因此未将某些租户替代应用于恶意软件和高可信度网络钓鱼。</span><span class="sxs-lookup"><span data-stu-id="3b580-111">Because Microsoft wants to keep our customers [secure by default](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions), some tenant overrides are not applied for malware and high confidence phishing.</span></span> <span data-ttu-id="3b580-112">这些替代包括：o   允许发件人列表或允许域列表（反垃圾邮件策略）o   Outlook 安全发件人 O   IP 允许列表（连接筛选）</span><span class="sxs-lookup"><span data-stu-id="3b580-112">These overrides include: o   Allowed sender lists or allowed domain lists (anti-spam policies) o   Outlook Safe Senders o   IP Allow List (connection filtering)</span></span> 
- <span data-ttu-id="3b580-113">允许高可信度钓鱼邮件绕过筛选的唯一替代是 Exchange 邮件流规则（也称为传输规则）。</span><span class="sxs-lookup"><span data-stu-id="3b580-113">The only override that allows high confidence phishing message to bypass filtering is Exchange mailflow rules (also known as transport rules).</span></span> <span data-ttu-id="3b580-114">若要使用邮件流规则绕过筛选，请参阅 **[使用邮件流规则来设置邮件中的垃圾邮件可信度级别 (SCL)](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**。</span><span class="sxs-lookup"><span data-stu-id="3b580-114">To use mail flow rules to bypass filtering, see **[Use mail flow rules to set the spam confidence level (SCL) in messages](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**.</span></span>