---
title: 打开邮箱审核
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: aa0ff925ae891d28e31394ec66eb17c2d9710008
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464471"
---
# <a name="turn-on-mailbox-auditing"></a>打开邮箱审核

若要为单个用户或整个组织启用邮箱审核，请从远程 PowerShell 运行以下 cmdlet：

- **单个用户**：Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
- **组织**：Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} |Set-Mailbox -AuditEnabled $true

若要了解更多信息，请参阅["管理邮箱审核"。](https://go.microsoft.com/fwlink/?linkid=2103668)