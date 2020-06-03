---
title: Outlook 网页版中的 S/MIME
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511498"
---
# <a name="encrypt-email-messages-in-outlook"></a>在 Outlook 中加密电子邮件

Microsoft 365 邮件加密是基于 Microsoft Azure 权限管理（Azure RMS）构建的，这是 Azure 信息保护的一部分。 如果你的订阅包括 Azure 权限管理或 Azure 信息保护，**则无需执行任何操作来手动启用或激活**权限管理服务。

根据客户反馈，我们将不再启用 Exchange 邮件流规则，以在默认情况下，在租户中自动对包含特定类型敏感信息的出站电子邮件进行加密。 相反，我们将提供有关如何进行此操作的详细说明。 有关如何创建传输规则以加密敏感信息的其他详细信息，请参阅[本文](https://aka.ms/OmeEtr)。

- 如果使用 Web 上的 Outlook （以前称为**OWA**）：撰写电子邮件时，只需在 OWA 中单击 "**保护**" 即可。 这将应用 "不转发" 权限。 单击 "**更改权限**"，然后选择 "**加密**" 仅加密邮件。

- 如果使用**outlook 客户端**：从 outlook 2013 或2016发送加密邮件，或 outlook 2016 for Mac，请选择 "**选项**  >  **权限**"，然后选择所需的保护选项。

- 若要自动对发送给特定收件人或外部合作伙伴组织的**所有电子邮件进行加密**，需要在 Exchange 管理中心中创建邮件流传输规则。 [本支持文章](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)中提供了详细说明。

