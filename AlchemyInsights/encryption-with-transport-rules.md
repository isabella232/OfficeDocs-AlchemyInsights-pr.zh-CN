---
title: 使用传输规则进行加密
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: 4c43fc16db84832c4e2aa3b6483632de6861b877
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784333"
---
# <a name="encryption-with-transport-rules"></a>使用传输规则进行加密

在 [Exchange 管理中心](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) 中，可使用邮件流规则中的 Office 邮件加密 (OME) 功能来触发邮件加密。 选择“传输规则”条件上的“**应用 Office 365 邮件加密和权限保护**”选项。

- 有关详细信息，请参阅[定义用于加密的邮件流规则](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)。

- 在 Powershell 中，使用 [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet 并将 *ApplyOME* 参数设置为 $true。
