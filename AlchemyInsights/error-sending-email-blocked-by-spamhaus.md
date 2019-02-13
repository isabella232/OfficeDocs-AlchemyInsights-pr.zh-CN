---
title: 发送电子邮件被 SpamHaus 错误
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 249f16d057b0539d71dc514ac35df28ab78fa061
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912338"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="9331b-102">发送电子邮件的错误： 使用 Spamhaus 阻止的客户端主机</span><span class="sxs-lookup"><span data-stu-id="9331b-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="9331b-p101">在阻止列表由[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)拥有发送消息的 IP 地址。Spamhaus 被阻止的原因包括受到攻击的帐户，威胁机共享一个公用 IP 地址，以及 Internet 服务提供程序 (ISP) 策略。可能的修复方法是：</span><span class="sxs-lookup"><span data-stu-id="9331b-p101">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies. Possible fixes are:</span></span>
  
- <span data-ttu-id="9331b-106">阻止到其中控制源电子邮件服务器的 Office 365 的入站邮件，您需要确定原因并从 Spamhaus 网站中移除块。</span><span class="sxs-lookup"><span data-stu-id="9331b-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="9331b-p102">阻止到源 IP 地址其中给其他人所属的 Office 365 的入站邮件，地址所有者需要从 Spamhaus 网站中移除块。如果策略阻止列表 (PBL) 上的 IP 地址，所有者可以分配一个不同的静态 IP 地址或从 PBL 删除的地址。</span><span class="sxs-lookup"><span data-stu-id="9331b-p102">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website. If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="9331b-p103">从 Office 365 域阻止的出站邮件，您可以通过第三方服务路由的邮件如果收到此错误。WHOIS 查找工具可用于查找已阻止的 IP 地址所有者。</span><span class="sxs-lookup"><span data-stu-id="9331b-p103">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service. You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

