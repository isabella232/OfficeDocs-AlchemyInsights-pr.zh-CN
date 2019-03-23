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
ms.openlocfilehash: f44ed42906b85e63f1f694813f54710906969904
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2019
ms.locfileid: "30772432"
---
# <a name="winsock-error-10061"></a>Winsock 错误10061

此错误代码意味着 Office 365 无法建立与目标主机的 TCP 套接字 (连接)。 此错误最可能的原因是防火墙配置存在问题。 若要解决此问题, 请检查这些设置:
  
- 使用[Office 365 url 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)中的信息验证防火墙配置
    
- 如果错误是 exchange online protection (EOP) 所特有的, 则之前应该已通知[exchange online protection IP 地址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)发生了更改。
    
- 验证您的 Internet 服务提供商 (ISP) 是否未阻止该端口。
    
- 验证连接器中的智能主机和目标服务器设置。
    
请注意, Office 365 不会以这种方式阻止*传入*连接。 
  

