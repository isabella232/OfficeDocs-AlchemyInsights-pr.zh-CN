---
title: 使用传输规则进行加密
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: dfd77bc83b4b278e3630858f54fdfb109ade2a14
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813858"
---
# <a name="encryption-with-transport-rules"></a>使用传输规则进行加密

在 [Exchange 管理中心](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) 中，可使用邮件流规则中的 Office 邮件加密 (OME) 功能来触发邮件加密。 选择“传输规则”条件上的“**应用 Office 365 邮件加密和权限保护**”选项。

- 有关详细信息，请参阅[定义用于加密的邮件流规则](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)。

- 在 Powershell 中，使用 [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) cmdlet 并将 *ApplyOME* 参数设置为 $true。
