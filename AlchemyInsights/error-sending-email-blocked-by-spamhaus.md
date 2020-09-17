---
title: 发送 SpamHaus 阻止的电子邮件时出错
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783757"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>发送电子邮件时出错：已阻止使用 Spamhaus 的客户端主机

发送邮件的 IP 地址在 [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)所拥有的阻止列表中。 被 Spamhaus 阻止的原因包括受到危害的帐户、共享公共 IP 地址的计算机以及 Internet 服务提供商 (ISP) 策略。 可能的修补程序包括：
  
- 对于控制源电子邮件服务器的阻止的入站邮件，您需要确定原因并从 Spamhaus 网站中删除该阻止。

- 对于源 IP 地址属于其他人的阻止入站邮件，地址所有者需要从 Spamhaus 网站中删除该阻止。 如果 IP 地址在策略阻止列表中 (PBL) ，则所有者可以分配不同的静态 IP 地址，或从 PBL 中删除该地址。

- 对于连接到 Microsoft 的域中阻止的出站邮件，如果通过第三方服务路由邮件，则可能会收到此错误。 您可以使用 WHOIS 查找工具来查找阻止的 IP 地址所有者。
