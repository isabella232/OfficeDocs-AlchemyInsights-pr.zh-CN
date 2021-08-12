---
title: 你的用户是否收到恶意电子邮件
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
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: de8823253d60efcd38bfa96864c146a2cedc0537f6d0aa41de6dafc6c7debc03
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929187"
---
# <a name="did-your-users-receive-malicious-email"></a>你的用户是否收到恶意电子邮件？

- 现在，你可以使用[安全与合规中心中的“管理员提交”](https://sip.protection.office.com/reportsubmission)来 Microsoft 报告恶意电子邮件。

提交至 [管理员提交](https://sip.protection.office.com/reportsubmission)中的邮件将会被扫描，以下结果将显示在 **详细信息** 的弹出页面中：

- 发件人的电子邮件身份验证是否在发送时验证失败。
- 任何可能影响或覆盖邮件裁定的策略信息。
- 当前触发结果，以查看邮件中所包含的 URL 或文件是否是恶意的。
- 评价员的反馈

如果找到了覆盖，则应该会在数分钟内完成重新扫描。如果电子邮件身份验证中不存在问题，或者覆盖对递送没有影响，则可能需要最多一天的时间才能收到评价员的反馈。

如果不同意邮件、URL 或文件的最终裁定（被阻止与未阻止），请在一天之后再次提交该邮件以进行重新扫描。 再次提交邮件后，裁定更改的几率是相当高的。

同时，你可按照[本文](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)中的说明从用户的收件箱中删除恶意电子邮件。

- 使用 Microsoft Defender for Office 365 的客户可以：
    - 使用 [威胁资源管理器“查找”和”删除可疑电子邮件”](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [使用安全链接阻止访问](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links)恶意 URL
    - 跟踪已单击和已访问恶意 URL 的用户：[查看网络钓鱼 URL 并单击裁定数据](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - 手动[开始“自动调查”](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

你也可以按照[防范恶意 URL 和文件](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats)中的说明，保护自己免受恶意文件和 URL 的侵害。