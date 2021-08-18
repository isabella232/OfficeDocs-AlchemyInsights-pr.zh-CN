---
title: 阻止或取消阻止外部自动电子邮件转发
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
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315864"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>阻止或取消阻止自动电子邮件转发

若要为特定邮箱启用或禁用电子邮件转发，请参阅配置 [电子邮件转发](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)。

管理员可以使用出站垃圾邮件策略来控制 [组织的外部转发](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)。 您可以在 Microsoft 365 Defender PowerShell 中的 <https://security.microsoft.com/antispam> [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) cmdlet 或通过使用 Exchange Online 管理出站垃圾邮件策略。

如果您收到以下错误 **："550 5.7.520 访问** 被拒绝，您的组织不允许外部转发"，请确保将策略配置为启用外部自动转发的邮件。

**注意**：我们建议使用默认值 **Automatic - 系统控制** 默认出站垃圾邮件筛选策略中的"自动转发规则"设置， (自动外部转发被阻止;内部自动转发仍) 。 您应该创建自定义出站垃圾邮件筛选器策略，并使用值 On **- 仅** 对需要外部自动电子邮件转发的用户启用转发。 有关详细信息，请参阅[Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)。
