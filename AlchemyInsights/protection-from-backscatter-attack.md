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
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897535"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="dce45-102">防止退信式垃圾邮件攻击</span><span class="sxs-lookup"><span data-stu-id="dce45-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="dce45-103">退信式垃圾邮件是针对你未发送的邮件收到的未送达报告（也称为 NDR 或退回邮件）。</span><span class="sxs-lookup"><span data-stu-id="dce45-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="dce45-104">垃圾邮件发送者伪造（欺骗）邮件的 **发件人：** 地址，并且他们经常使用真实的电子邮件地址来增强邮件的信誉。</span><span class="sxs-lookup"><span data-stu-id="dce45-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="dce45-105">因此，当垃圾邮件发送者不可避免地将邮件发送给不存在的收件人时，实际上会诱使目标电子邮件服务器将 NDR 中无法送达的邮件退回给 **发件人：** 地址的伪造发件人。</span><span class="sxs-lookup"><span data-stu-id="dce45-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="dce45-106">有关其他信息，请参阅 [EOP 中的退信式垃圾邮件](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)。</span><span class="sxs-lookup"><span data-stu-id="dce45-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="dce45-107">**启用退信式垃圾邮件保护**</span><span class="sxs-lookup"><span data-stu-id="dce45-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="dce45-108">若要启用退信式垃圾邮件保护，请按照以下路径操作。</span><span class="sxs-lookup"><span data-stu-id="dce45-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="dce45-109">**protection.office.com >“威胁管理”>“策略”>“反垃圾邮件”>“选择垃圾邮件筛选策略并编辑策略”>“垃圾邮件属性”>“标记为垃圾邮件”>“NDR 退信式垃圾邮件”> 将其设置为“开”**</span><span class="sxs-lookup"><span data-stu-id="dce45-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="dce45-110">如果你认为帐户已被盗用，请参阅以下内容：</span><span class="sxs-lookup"><span data-stu-id="dce45-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="dce45-111">响应被盗用的电子邮件帐户</span><span class="sxs-lookup"><span data-stu-id="dce45-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="dce45-112">在 Office 365 中从“受限的用户”门户中删除被阻止的用户</span><span class="sxs-lookup"><span data-stu-id="dce45-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



