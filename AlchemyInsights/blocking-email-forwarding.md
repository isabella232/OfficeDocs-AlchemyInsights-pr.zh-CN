---
title: 726 阻止电子邮件转发
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059622"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>阻止或取消阻止电子邮件转发

若要为特定邮箱启用或禁用电子邮件转发，请参阅配置 [电子邮件转发](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)。

在租户级别，使用出站垃圾邮件策略完成对外部转发的控制。 你可以在此处通过安全与合规中心检查出站垃圾邮件筛选器策略，[](https://protection.office.com/antispam)或者使用[Get-HostedOutboundSpamFilterPolicy 命令检查出站垃圾邮件筛选器策略](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)。

如果您收到以下错误 **："550 5.7.520 访问** 被拒绝，您的组织不允许外部转发"，请确保将策略配置为启用外部自动转发。

**注意：** 建议在默认出站垃圾邮件筛选器策略上禁用"外部自动转发"，并仅为需要外部转发的用户启用它，方法为为这些用户创建自定义策略。 有关详细信息，请参阅在 Office 365[中配置外部电子邮件转发](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)。