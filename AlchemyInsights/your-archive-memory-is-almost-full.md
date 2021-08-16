---
title: 您的存档邮箱几乎已满
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046742"
---
# <a name="your-archive-mailbox-is-almost-full"></a>您的存档邮箱几乎已满

如果用户收到警告; **您的存档邮箱几乎已满**，或者您需要增加存档邮箱的大小，以下是一些提示：

1. 如果为用户分配了Exchange Online计划 1，请Exchange Online计划 **2** 许可证，以将大小从 50 GB 增加至 100GB。
1. 如果用户已分配有以下任一项：Exchange Online **计划 2** 或具有 Exchange Online Archiving 加载项的 Exchange Online 计划 1，请使用以下步骤启用自动扩展存档：。
 
    1. [连接到 Exchange Online Powershell 。](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true)
    2. 为用户运行以下命令let：  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. 运行以下命令let 以确认为用户启用该命令：  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

有关更多信息，请参阅：

- [启用无限制存档 - 管理员帮助 - Microsoft 365合规性|Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online限制 - 服务说明|Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [升级到其他业务计划|Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

