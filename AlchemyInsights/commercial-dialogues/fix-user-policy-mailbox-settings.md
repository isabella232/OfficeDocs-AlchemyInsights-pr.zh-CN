---
title: 修复用户策略/邮箱设置
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736151"
---
# <a name="fix-user-policymailbox-settings"></a>修复用户策略/邮箱设置

邮箱上的垃圾邮件设置影响此邮件。 若要查看设置，请执行下列操作：

1. 启动 Exchange 命令行管理程序。 有关详细信息，请参阅[Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432)。
2. 使用用户 (电子邮件地址运行此命令  **) ：get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. 检查发件人的电子邮件地址是 **TrustedSendersAndDomains** 还是 **BlockedSendersAndDomains 的一部分**。 如果电子邮件地址位于其中一个列表中，您可能需要将其删除。 若要了解更多信息，请参阅 [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047)。
