---
title: 1554 Winsock 错误10061
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
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698852"
---
# <a name="winsock-error-10061"></a>Winsock 错误10061

此错误代码表示 Microsoft 无法建立与目标主机的 TCP 套接字 (连接) 。 此错误最可能的原因是防火墙配置存在问题。 若要解决此问题，请检查这些设置：

- 使用[Microsoft 365 url 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)中的信息验证防火墙配置

- 如果错误是 Exchange Online Protection (EOP) 所特有的，则之前应该已通知 [Exchange Online PROTECTION IP 地址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)发生了更改。

- 确认 Internet 服务提供商 (ISP) 未阻止该端口。

- 验证连接器中的智能主机和目标服务器设置。

请注意，Microsoft 365 不会以这种方式阻止 *传入* 连接。
