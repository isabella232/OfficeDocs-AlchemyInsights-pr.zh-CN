---
title: 1554 Winsock 错误 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083220"
---
# <a name="winsock-error-10061"></a>Winsock 错误 10061

此错误代码意味着 Microsoft 无法建立 TCP 套接字 (与) 建立连接。 导致此错误的最可能原因是防火墙配置有问题。 若要解决此问题，请检查以下设置：

- 使用 URL 和 IP 地址范围内Microsoft 365[验证防火墙配置](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- 如果错误特定于 EOP Exchange Online Protection (，) ，则之前应该会通知您对 EOP IP 地址Exchange Online Protection[更改](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)。

- 验证 Internet 服务提供商 (ISP) 未阻止端口。

- 验证连接器中的智能主机和目标服务器设置。

请注意Microsoft 365不会阻止 *此方式的* 传入连接。
