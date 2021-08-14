---
title: 反垃圾邮件 - 5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: cb9073306c65b09813290d6c8470d14395d2836fa3048f8ce0ecb8b06e71a010
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932159"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>修复错误代码为 5.7.23 的电子邮件传递问题

在 Web 上公开提供的 SPF 或 DNS 记录检查器中验证域的 SPF DNS 记录。

确认 Microsoft 未将出站邮件标识为垃圾邮件，并通过高风险传递池 [进行路由](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)。 高风险传递池中的邮件无法通过 SPF 检查，因此目标电子邮件组织不会接受。

如果问题仍然存在，您可能需要联系尝试发送电子邮件的邮件主机的管理员。 记下退回邮件中提供的详细外部错误。 Microsoft 支持可能无法进一步提供帮助。
