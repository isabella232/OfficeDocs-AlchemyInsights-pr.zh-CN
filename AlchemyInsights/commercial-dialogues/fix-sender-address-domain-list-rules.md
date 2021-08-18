---
title: 修复发件人地址/域列表规则
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
ms.openlocfilehash: 7e3c729e9bf630fa798c746f25f046606a1459a1
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320479"
---
# <a name="fix-sender-addressdomain-list-rules"></a>修复发件人地址/域列表规则

您的一个反垃圾邮件策略影响此邮件。 在"允许"或"阻止"列表中找到邮件的发件人。 若要查看策略，请执行以下步骤：

1. In the Microsoft 365 Defender portal at <https://security.microsoft.com/> ， go to Email & **Collaboration** Policies \> **& Rules** \> **Threat policies** \> **Anti-spam** in the **Policies** section.

   若要直接转到“**反垃圾邮件策略**”页面，请使用 <https://security.microsoft.com/antispam>。

2. 在 **"反垃圾邮件** (策略"页上，单击策略名称"类型为自定义反垃圾邮件策略"或"名称为反垃圾邮件入站策略" (**默认** 策略) ) 。
3. 在出现的详细信息飞出控件中，选择"允许和阻止的发件人和域"部分中的"编辑允许和阻止的发件人 **和** 域"。
4. 在" **允许** "部分，单击"管理发件人"或" **允许域 \<nn\>** "，查看发件人 **和域**。

有关详细信息，请参阅[在 EOP 中配置反垃圾邮件策略](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)。
