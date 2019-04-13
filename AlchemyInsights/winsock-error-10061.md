---
title: 1554 Winsock 错误10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7651effc43cb0c4bc2fbbe5349bb72303943f493
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859130"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="0ae27-102">Winsock 错误10061</span><span class="sxs-lookup"><span data-stu-id="0ae27-102">Winsock error 10061</span></span>

<span data-ttu-id="0ae27-103">此错误代码意味着 Office 365 无法建立与目标主机的 TCP 套接字 (连接)。</span><span class="sxs-lookup"><span data-stu-id="0ae27-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="0ae27-104">此错误最可能的原因是防火墙配置存在问题。</span><span class="sxs-lookup"><span data-stu-id="0ae27-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="0ae27-105">若要解决此问题, 请检查这些设置:</span><span class="sxs-lookup"><span data-stu-id="0ae27-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="0ae27-106">使用[Office 365 url 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)中的信息验证防火墙配置</span><span class="sxs-lookup"><span data-stu-id="0ae27-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="0ae27-107">如果错误是 exchange online protection (EOP) 所特有的, 则之前应该已通知[exchange online protection IP 地址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)发生了更改。</span><span class="sxs-lookup"><span data-stu-id="0ae27-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="0ae27-108">验证您的 Internet 服务提供商 (ISP) 是否未阻止该端口。</span><span class="sxs-lookup"><span data-stu-id="0ae27-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="0ae27-109">验证连接器中的智能主机和目标服务器设置。</span><span class="sxs-lookup"><span data-stu-id="0ae27-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="0ae27-110">请注意, Office 365 不会以这种方式阻止*传入*连接。</span><span class="sxs-lookup"><span data-stu-id="0ae27-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>
