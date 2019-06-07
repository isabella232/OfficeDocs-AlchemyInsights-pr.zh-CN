---
title: 1554 Winsock 错误10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 3fa3b2f2e10d3ebe480861e1f2d7ecaa262afe14
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757071"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="3eb9a-102">Winsock 错误10061</span><span class="sxs-lookup"><span data-stu-id="3eb9a-102">Winsock error 10061</span></span>

<span data-ttu-id="3eb9a-103">此错误代码意味着 Office 365 无法建立与目标主机的 TCP 套接字 (连接)。</span><span class="sxs-lookup"><span data-stu-id="3eb9a-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="3eb9a-104">此错误最可能的原因是防火墙配置存在问题。</span><span class="sxs-lookup"><span data-stu-id="3eb9a-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="3eb9a-105">若要解决此问题, 请检查这些设置:</span><span class="sxs-lookup"><span data-stu-id="3eb9a-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="3eb9a-106">使用[Office 365 url 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)中的信息验证防火墙配置</span><span class="sxs-lookup"><span data-stu-id="3eb9a-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="3eb9a-107">如果错误是 Exchange Online Protection (EOP) 所特有的, 则之前应该已通知[Exchange Online PROTECTION IP 地址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)发生了更改。</span><span class="sxs-lookup"><span data-stu-id="3eb9a-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="3eb9a-108">验证您的 Internet 服务提供商 (ISP) 是否未阻止该端口。</span><span class="sxs-lookup"><span data-stu-id="3eb9a-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="3eb9a-109">验证连接器中的智能主机和目标服务器设置。</span><span class="sxs-lookup"><span data-stu-id="3eb9a-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="3eb9a-110">请注意, Office 365 不会以这种方式阻止*传入*连接。</span><span class="sxs-lookup"><span data-stu-id="3eb9a-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>
