---
title: 发送电子邮件被 SpamHaus 错误
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29459207"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>发送电子邮件的错误： 使用 Spamhaus 阻止的客户端主机

在阻止列表由[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)拥有发送消息的 IP 地址。Spamhaus 被阻止的原因包括受到攻击的帐户，威胁机共享一个公用 IP 地址，以及 Internet 服务提供程序 (ISP) 策略。可能的修复方法是：
  
- 阻止到其中控制源电子邮件服务器的 Office 365 的入站邮件，您需要确定原因并从 Spamhaus 网站中移除块。
    
- 阻止到源 IP 地址其中给其他人所属的 Office 365 的入站邮件，地址所有者需要从 Spamhaus 网站中移除块。如果策略阻止列表 (PBL) 上的 IP 地址，所有者可以分配一个不同的静态 IP 地址或从 PBL 删除的地址。
    
- 从 Office 365 域阻止的出站邮件，您可以通过第三方服务路由的邮件如果收到此错误。WHOIS 查找工具可用于查找已阻止的 IP 地址所有者。
    

