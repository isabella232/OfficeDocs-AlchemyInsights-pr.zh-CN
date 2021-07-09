---
title: 出站中继池
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53339956"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="1b66c-102">出站中继池</span><span class="sxs-lookup"><span data-stu-id="1b66c-102">Outbound relay pool</span></span>

<span data-ttu-id="1b66c-103">Microsoft 正在对配置进行一些更改，以通过 Microsoft 365 中继或转发Microsoft 365。</span><span class="sxs-lookup"><span data-stu-id="1b66c-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="1b66c-104">在某些情况下，邮件使用特殊的中继池通过 Microsoft 365转发或中继。</span><span class="sxs-lookup"><span data-stu-id="1b66c-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="1b66c-105">使用中继池发送的邮件最终可能位于收件人的垃圾邮件文件夹中。</span><span class="sxs-lookup"><span data-stu-id="1b66c-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="1b66c-106">有关详细信息，请参阅出 [站传递池](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="1b66c-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="1b66c-107">为了避免使用中继池的情况，请确保转发/中继邮件满足以下条件之一：</span><span class="sxs-lookup"><span data-stu-id="1b66c-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="1b66c-108">出站发件人是租户的接受域。</span><span class="sxs-lookup"><span data-stu-id="1b66c-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="1b66c-109">发件人策略 (SPF) 在邮件发送到邮件时通过Microsoft 365。</span><span class="sxs-lookup"><span data-stu-id="1b66c-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="1b66c-110">当邮件发送到 (时) P2 发件人域中的域密钥标识的邮件和 DKIM Microsoft 365。</span><span class="sxs-lookup"><span data-stu-id="1b66c-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="1b66c-111">满足上述条件的邮件不会通过中继池中继。</span><span class="sxs-lookup"><span data-stu-id="1b66c-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="1b66c-112">如果域的 MX 记录指向第三方或本地服务器，请使用增强的筛选，以确保 SPF 验证对入站电子邮件正确无误，并避免通过中继池发送电子邮件。</span><span class="sxs-lookup"><span data-stu-id="1b66c-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="1b66c-113">**如何判断中继池是否受到影响？**</span><span class="sxs-lookup"><span data-stu-id="1b66c-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="1b66c-114">如果转发或中继的电子邮件使用上述条件之一，则邮件不会通过中继池中继。</span><span class="sxs-lookup"><span data-stu-id="1b66c-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="1b66c-115">但是，如果邮件通过中继池发送，则出站服务器 IP 在 40.95.0.0/16 范围内，出站服务器名称将 **rly** 包括在名称中。</span><span class="sxs-lookup"><span data-stu-id="1b66c-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

