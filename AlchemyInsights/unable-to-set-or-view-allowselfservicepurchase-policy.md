---
title: 无法设置或查看 AllowSelfServicePurchase 策略
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 255dbe35b808b3fe6b5707779251bf3f4a7e1c269c8b6f0ac2cb43ca03c469e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020182"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a>无法设置或查看 AllowSelfServicePurchase 策略

尝试设置或查看 AllowSelfServicePurchase 策略时，会收到以下错误消息：

*HandleError：检索 PolicyId 为"AllowSelfServicePurchase"的产品策略失败，ErrorMessage - 基础连接已关闭：发送时发生意外错误。*

这可能是由于传输层安全性的较旧版本 (TLS) 。 若要连接 MSCommerce 服务，您需要使用 TLS 1.2 或更大。  

尝试以下步骤以启用/将 TLS 协议设置为 1.2、验证并重试。
 1. 在 PowerShell 命令提示符 (PS C：输入以下命令以将 \) TLS 协议设置为版本 1.2：

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. 使用以下命令 (TLS) 使用中的 TLS 协议：

    `[Net.ServicePointManager]::SecurityProtocol` 

3. 根据需要重试"获取"或"更新"命令。

