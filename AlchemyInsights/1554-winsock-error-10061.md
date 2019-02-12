---
title: 1554 Winsock 错误 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903086"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="e7af5-102">Winsock 错误 10061</span><span class="sxs-lookup"><span data-stu-id="e7af5-102">Winsock error 10061</span></span>

<span data-ttu-id="e7af5-p101">此错误代码表示 Office 365 无法建立与目标主机的 TCP 套接字 （连接）。此错误的最可能的原因是您的防火墙配置问题。若要解决此问题，请检查这些设置：</span><span class="sxs-lookup"><span data-stu-id="e7af5-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="e7af5-106">验证[Office 365 Url 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)中的信息与防火墙配置</span><span class="sxs-lookup"><span data-stu-id="e7af5-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="e7af5-107">如果错误是特定到 Exchange Online Protection (EOP)，您应该已经以前通知到[Exchange Online Protection IP 地址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的更改。</span><span class="sxs-lookup"><span data-stu-id="e7af5-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="e7af5-108">确认您 Internet 服务提供程序 (ISP) 不阻止端口。</span><span class="sxs-lookup"><span data-stu-id="e7af5-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="e7af5-109">确认您连接器中的智能主机和目标服务器设置。</span><span class="sxs-lookup"><span data-stu-id="e7af5-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="e7af5-110">请注意，Office 365 不阻止这种方式*传入*连接。</span><span class="sxs-lookup"><span data-stu-id="e7af5-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

