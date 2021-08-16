---
title: 启用邮箱审核
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
ms.openlocfilehash: 797dd57aaa43e879c015a36c79c8c9fb13e04ae894b33b0f7c6d9694d1ae1960
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058028"
---
# <a name="turn-on-mailbox-auditing"></a>启用邮箱审核

若要为单个用户或整个组织启用邮箱审核，请从远程 PowerShell 运行以下 cmdlet：

- **单个用户**：Set-Mailbox -Identity "Jane Dow" -AuditEnabled $true
- **组织**：Get-Mailbox -ResultSize Unlimited -Filter {RecipientTypeDetails -eq "UserMailbox"} |Set-Mailbox -AuditEnabled $true

若要了解更多信息，请参阅 [管理邮箱审核](https://go.microsoft.com/fwlink/?linkid=2103668)。