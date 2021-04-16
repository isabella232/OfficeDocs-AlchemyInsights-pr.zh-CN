---
title: 发送由 Spam在垃圾邮件中阻止的电子邮件时出错
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813714"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="0fdf2-102">发送电子邮件时出错：使用 Spam在客户端主机上被阻止</span><span class="sxs-lookup"><span data-stu-id="0fdf2-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="0fdf2-103">发送邮件的 IP 地址位于 Spam用户拥有的阻止 [列表中](https://go.microsoft.com/fwlink/p/?linkid=123245)。</span><span class="sxs-lookup"><span data-stu-id="0fdf2-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="0fdf2-104">垃圾邮件阻止的原因包括帐户遭到入侵、共享公用 IP 地址的计算机遭到入侵以及 INTERNET 服务提供商 (ISP) 策略。</span><span class="sxs-lookup"><span data-stu-id="0fdf2-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="0fdf2-105">可能的修补程序包括：</span><span class="sxs-lookup"><span data-stu-id="0fdf2-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="0fdf2-106">对于控制源电子邮件服务器的阻止入站邮件，您需要确定原因并从 Spam用户网站中删除此阻止。</span><span class="sxs-lookup"><span data-stu-id="0fdf2-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="0fdf2-107">对于源 IP 地址属于其他人的阻止入站邮件，地址所有者需要从 Spam用户网站中删除此阻止。</span><span class="sxs-lookup"><span data-stu-id="0fdf2-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="0fdf2-108">如果 IP 地址位于 PBL 策略策略 (列表中) ，则所有者可以分配其他静态 IP 地址，或者从 PBL 中删除该地址。</span><span class="sxs-lookup"><span data-stu-id="0fdf2-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="0fdf2-109">对于从连接到 Microsoft 的域阻止的出站邮件，如果邮件通过第三方服务路由，则会收到此错误。</span><span class="sxs-lookup"><span data-stu-id="0fdf2-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="0fdf2-110">可以使用 WHOIS 查找工具查找阻止的 IP 地址所有者。</span><span class="sxs-lookup"><span data-stu-id="0fdf2-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
