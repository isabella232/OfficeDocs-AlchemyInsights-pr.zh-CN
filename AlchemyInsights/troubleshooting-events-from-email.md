---
title: 来自电子邮件的事件的疑难解答
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834829"
---
# <a name="troubleshooting-events-from-email"></a>来自电子邮件的事件的疑难解答

1. 验证是否已为邮箱启用该功能：**Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. 然后查看“来自电子邮件的事件”日志 **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. 在“来自电子邮件的事件”日志中，找到与邮箱中的相应项目匹配的 InternetMessageId。  

4. TrustScore 决定是否添加该项目。 仅当 TrustScore =“Trusted”时才会添加事件。

TrustScore 由 SPF、Dkim 或 Dmarc 属性决定，它们位于邮件头中。

若要查看这些属性，请执行以下操作：

**桌面版 Outlook**

- 打开相应项目
- “文件”->“属性”->“Internet 邮件头”

或

**MFCMapi**

- 导航到收件箱中的相应项目
- 查找 PR_TRANSPORT_MESSAGE_HEADERS_W

系统将在传输和路由过程中确定并记录这些属性。 如需进一步进行故障排除，可能需要跟进有关 SPF、DKIM 和 DMARC 中故障的传输支持。