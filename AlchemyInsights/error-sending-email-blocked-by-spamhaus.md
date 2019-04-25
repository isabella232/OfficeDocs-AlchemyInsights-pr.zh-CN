---
title: 发送 SpamHaus 阻止的电子邮件时出错
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402249"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="6f9a2-102">发送电子邮件时出错: 已阻止使用 Spamhaus 的客户端主机</span><span class="sxs-lookup"><span data-stu-id="6f9a2-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="6f9a2-103">发送邮件的 IP 地址在[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)所拥有的阻止列表中。</span><span class="sxs-lookup"><span data-stu-id="6f9a2-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="6f9a2-104">被 Spamhaus 阻止的原因包括已损坏的帐户、共享公共 IP 地址的受损计算机以及 Internet 服务提供商 (ISP) 策略。</span><span class="sxs-lookup"><span data-stu-id="6f9a2-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="6f9a2-105">可能的修补程序包括:</span><span class="sxs-lookup"><span data-stu-id="6f9a2-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="6f9a2-106">对于控制源电子邮件服务器的 Office 365 的已阻止入站邮件, 您需要确定原因并从 Spamhaus 网站中删除该阻止。</span><span class="sxs-lookup"><span data-stu-id="6f9a2-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="6f9a2-107">对于阻止的入站邮件到 Office 365, 其中源 IP 地址属于其他人, 地址所有者需要从 Spamhaus 网站中删除该阻止。</span><span class="sxs-lookup"><span data-stu-id="6f9a2-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="6f9a2-108">如果 IP 地址在策略阻止列表 (PBL) 上, 则所有者可以分配不同的静态 IP 地址, 或从 PBL 中删除该地址。</span><span class="sxs-lookup"><span data-stu-id="6f9a2-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="6f9a2-109">对于 Office 365 域中阻止的出站邮件, 如果通过第三方服务路由邮件, 则可能会收到此错误。</span><span class="sxs-lookup"><span data-stu-id="6f9a2-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="6f9a2-110">您可以使用 WHOIS 查找工具来查找阻止的 IP 地址所有者。</span><span class="sxs-lookup"><span data-stu-id="6f9a2-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

