---
title: 无法设置或查看 AllowSelfServicePurchase 策略
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158550"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>无法设置或查看 AllowSelfServicePurchase 策略

在尝试设置或查看 AllowSelfServicePurchase 策略时，您会收到以下错误消息：

*HandleError：无法检索带有 PolicyId "AllowSelfServicePurchase" 的产品策略，错误-基础连接已关闭：发送时发生意外错误。*

这可能是由于较旧版本的传输层安全性（TLS）造成的。 若要连接 MSCommerce 服务，您需要使用 TLS 1.2 或更高版本。  

尝试执行以下步骤，将 TLS 协议启用/设置为1.2、验证和重试。
 1. 在 PowerShell 命令提示符（PS C：\) ）中，输入以下命令，将 TLS 协议设置为版本1.2：

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. 使用以下命令验证所使用的 TLS 协议：

    `[Net.ServicePointManager]::SecurityProtocol` 

3. 根据需要，重试 Get 或 Update 命令。

