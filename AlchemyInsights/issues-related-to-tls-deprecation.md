---
title: 由于 TLS 1.0 和 TLS 1.1 禁用Office 365发送/接收电子邮件
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054896"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>由于 TLS 1.0 和 TLS 1.1 禁用Office 365发送/接收电子邮件

正如消息中心文章 MC229914 所确认的，TLS 1.0 和 TLS 1.1 弃用开始强制Exchange Online邮件流终结点。 很快Office 365不再接受来自外部源的 TLS 1.0 和 TLS 1.1 电子邮件连接。 此外，Exchange Online永远不会使用 TLS 1.0 或 1.1 发送出站电子邮件。 如果由于 TLS 1.0 或 1.1 禁用而面临问题，可能会遇到以下错误之一：

- 发件人收到 NDR 退回 -"421 4.4.2 连接由于 SocketError 而丢弃"
- 向 Officer 365 发送电子邮件的本地服务器的队列查看器中出现错误- "421 4.4.2 连接由于 SocketError"而中断
- 向客户端发送电子邮件[的](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging)服务器的发送连接器协议日志中Office 365- TLS 协商失败，出现错误 SocketError
- 发送或接收连接器协议日志中出现错误 - '451 5.7.3 必须先发出 STARTTLS 命令'

如果遇到上述任何错误，请检查以下注册表项，确保发送或接收电子邮件的服务器已启用 TLS 1.2：

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2][HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword：000000000 "Enabled"=dword：00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword：000000000 "Enabled"=dword：00000001**

如果对上述注册表项进行任何更改以启用 TLS 1.2，请重新启动服务器以使更改生效。 此外，请确保已安装最新的 Windows Exchange 更新。

有关详细信息，请参阅：

- [Exchange ServerTLS 指南第 1 部分：为 TLS 1.2 做好准备 - Microsoft 技术Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange ServerTLS 指南第 2 部分：启用 TLS 1.2 和标识未使用它的客户端 - Microsoft Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [了解电子邮件方案（如果无法在 TLS 版本之间达成一致Exchange Online - Microsoft 技术Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
