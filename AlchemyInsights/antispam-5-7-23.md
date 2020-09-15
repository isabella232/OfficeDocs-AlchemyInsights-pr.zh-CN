---
title: 反垃圾邮件-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717315"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>修复错误代码5.7.23 的电子邮件传递问题

在 web 上的公开发布的 SPF 或 DNS 记录检查器中验证您的域的 SPF DNS 记录。

确认出站邮件未被 Microsoft 标识为 "垃圾邮件"，并通过 [高风险传递池](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)进行路由。 高风险传递池中的邮件不会通过 SPF 检查，因此目标电子邮件组织不接受这些邮件。

如果问题仍然存在，则可能需要联系您尝试向其发送电子邮件的邮件主机的管理员。 记下弹跳消息中提供的详细外部错误。 Microsoft 支持可能无法进一步协助。
