---
title: Outlook 网页版中的 S/MIME
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010714"
---
# <a name="encrypt-email-messages-in-outlook"></a>加密电子邮件Outlook

Microsoft 365邮件加密基于 Azure RMS Microsoft Azure权限 (，) Azure 信息保护的一部分。 如果你的订阅包含 Azure 权限管理或 Azure 信息保护，则无需执行任何操作即可 **手动启用或** 激活权限管理服务。

根据客户反馈，我们将不再启用Exchange规则自动加密包含特定类型敏感信息的出站电子邮件。 相反，我们提供了有关如何执行这些操作的详细说明。 若要详细了解如何创建传输规则来加密敏感信息，请参阅 [本文](https://aka.ms/OmeEtr)。

- If using Outlook on the Web (formerly **OWA**) ： When composing an email message， simply click **Protect** in OWA. 这将应用"不要转发"权限。 单击 **"更改权限** "， **然后选择"加密** "以仅加密邮件。

- 如果使用 **Outlook 客户端**：若要从 Outlook 2013 或 2016 或 Outlook 2016 for Mac 发送加密邮件，请选择"选项权限"，然后选择所需的保护  >  选项。

- 若要 **自动加密发送给特定** 收件人或外部合作伙伴组织的所有电子邮件，您需要在管理中心内创建Exchange传输规则。 此支持文章中 [提供了详细说明](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)。

