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
# <a name="winsock-error-10061"></a>Winsock 错误 10061

此错误代码表示 Office 365 无法建立与目标主机的 TCP 套接字 （连接）。此错误的最可能的原因是您的防火墙配置问题。若要解决此问题，请检查这些设置：
  
- 验证[Office 365 Url 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)中的信息与防火墙配置
    
- 如果错误是特定到 Exchange Online Protection (EOP)，您应该已经以前通知到[Exchange Online Protection IP 地址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的更改。
    
- 确认您 Internet 服务提供程序 (ISP) 不阻止端口。
    
- 确认您连接器中的智能主机和目标服务器设置。
    
请注意，Office 365 不阻止这种方式*传入*连接。 
  

