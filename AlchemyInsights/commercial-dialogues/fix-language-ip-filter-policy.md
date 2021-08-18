---
title: 修复语言/IP 筛选器策略
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
ms.openlocfilehash: 25744bee6f3ed06ae67fc3c246c7d64fce9994bb
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320515"
---
# <a name="fix-languageip-filter-policy"></a>修复语言/IP 筛选器策略

您的一个反垃圾邮件策略影响此邮件。 若要查看策略，请执行以下步骤：

1. In the Microsoft 365 Defender portal at <https://security.microsoft.com/> ， go to Email & **Collaboration** Policies \> **& Rules** \> **Threat policies** \> **Anti-spam** in the **Policies** section.

   若要直接转到“**反垃圾邮件策略**”页面，请使用 <https://security.microsoft.com/antispam>。

2. 在 **"反垃圾邮件** (策略"页上，单击策略名称"类型为自定义反垃圾邮件策略"或"名称为反垃圾邮件入站策略" (**默认** 策略) ) 。
3. In the details flyout that appears， select **Edit spam threshold and properties** in the Bulk email threshold & spam **properties** section.
4. 在" **标记为垃圾邮件"** 部分，查看" **包含特定语言"和** " **来自这些国家/地区"** 设置。

有关详细信息，请参阅[在 EOP 中配置反垃圾邮件策略](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)。
