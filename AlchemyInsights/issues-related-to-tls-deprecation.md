---
title: 由于 TLS 1.0 和 TLS 1.1 禁用，无法向 Office 365 发送/接收电子邮件
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
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50726911"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="fc00f-102">由于 TLS 1.0 和 TLS 1.1 禁用，无法向 Office 365 发送/接收电子邮件</span><span class="sxs-lookup"><span data-stu-id="fc00f-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="fc00f-103">正如消息中心文章 MC229914 所确认的，TLS 1.0 和 TLS 1.1 弃用开始对 Exchange Online 邮件流终结点强制执行。</span><span class="sxs-lookup"><span data-stu-id="fc00f-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="fc00f-104">很快 Office 365 将不再接受来自外部源的 TLS 1.0 和 TLS 1.1 电子邮件连接。</span><span class="sxs-lookup"><span data-stu-id="fc00f-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="fc00f-105">此外，Exchange Online 绝不会使用 TLS 1.0 或 1.1 发送出站电子邮件。</span><span class="sxs-lookup"><span data-stu-id="fc00f-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="fc00f-106">如果由于 TLS 1.0 或 1.1 禁用而面临问题，可能会遇到以下错误之一：</span><span class="sxs-lookup"><span data-stu-id="fc00f-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="fc00f-107">发件人收到 NDR 退回 -"421 4.4.2 连接由于 SocketError 而丢弃"</span><span class="sxs-lookup"><span data-stu-id="fc00f-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="fc00f-108">向 Officer 365 发送电子邮件的本地服务器的队列查看器中出现错误- "421 4.4.2 连接由于 SocketError"而中断</span><span class="sxs-lookup"><span data-stu-id="fc00f-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="fc00f-109">向 Office [](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) 365 发送电子邮件的服务器上发送连接器协议日志中出现错误- TLS 协商失败，出现错误 SocketError</span><span class="sxs-lookup"><span data-stu-id="fc00f-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="fc00f-110">发送或接收连接器协议日志中出现错误 - '451 5.7.3 必须先发出 STARTTLS 命令'</span><span class="sxs-lookup"><span data-stu-id="fc00f-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="fc00f-111">如果遇到上述任何错误，请检查以下注册表项，确保发送或接收电子邮件的服务器已启用 TLS 1.2：</span><span class="sxs-lookup"><span data-stu-id="fc00f-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="fc00f-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2][HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword：000000000 "Enabled"=dword：00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword：0000000000 "Enabled"=dword：000000001**</span><span class="sxs-lookup"><span data-stu-id="fc00f-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="fc00f-113">如果对上述注册表项进行任何更改以启用 TLS 1.2，请重新启动服务器以使更改生效。</span><span class="sxs-lookup"><span data-stu-id="fc00f-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="fc00f-114">此外，请确保已安装最新的 Windows 和 Exchange 更新。</span><span class="sxs-lookup"><span data-stu-id="fc00f-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="fc00f-115">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="fc00f-115">For more information, see:</span></span>

- [<span data-ttu-id="fc00f-116">Exchange Server TLS 指南的第 1 部分：为 TLS 1.2 做好准备 - Microsoft 技术社区</span><span class="sxs-lookup"><span data-stu-id="fc00f-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="fc00f-117">Exchange Server TLS 指南第 2 部分：启用 TLS 1.2 和标识未使用它的客户端 - Microsoft 技术社区</span><span class="sxs-lookup"><span data-stu-id="fc00f-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="fc00f-118">了解无法在 Exchange Online 中就 TLS 版本达成一致的电子邮件方案 - Microsoft 技术社区</span><span class="sxs-lookup"><span data-stu-id="fc00f-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
