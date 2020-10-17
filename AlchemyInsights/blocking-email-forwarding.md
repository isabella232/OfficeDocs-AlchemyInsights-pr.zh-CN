---
title: 726阻止电子邮件转发
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478343"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>阻止或取消阻止电子邮件转发

若要启用或禁用特定邮箱的电子邮件转发，请参阅 [配置电子邮件转发](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)。

在租户级别，使用出站垃圾邮件策略来控制外部转发。 您可以从 "安全与 [合规中心"](https://protection.office.com/antispam) 中查看出站垃圾邮件筛选器策略，或使用 [HostedOutboundSpamFilterPolicy 命令](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)。

如果您遇到以下错误： **"550 5.7.520 访问被拒绝，您的组织不允许外部转发"**，请确保将策略配置为启用外部自动转发。

**注意：** 建议将外部 Autoforward 禁用默认的出站垃圾邮件筛选器策略，并仅为需要外部转发的用户启用这些用户的自定义策略，并对其启用。 若要了解详细信息，请参阅在 [Office 365 中配置外部电子邮件转发](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)。