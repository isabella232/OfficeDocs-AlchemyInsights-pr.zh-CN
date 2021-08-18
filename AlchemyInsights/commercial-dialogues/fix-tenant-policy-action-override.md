---
title: '修复租户策略 (替代) '
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
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326787"
---
# <a name="fix-tenant-policy-action-override"></a>修复租户策略 (替代) 

您的一个反垃圾邮件策略影响此邮件。 若要查看策略，请执行以下步骤：

1. In the Microsoft 365 Defender portal at <https://security.microsoft.com/> ， go to Email & **Collaboration** Policies \> **& Rules** \> **Threat policies** \> **Anti-spam** in the **Policies** section.

   若要直接转到“**反垃圾邮件策略**”页面，请使用 <https://security.microsoft.com/antispam>。

2. 在 **"反垃圾邮件** (策略"页上，单击策略名称"类型为自定义反垃圾邮件策略"或"名称为反垃圾邮件入站策略" (**默认** 策略) ) 。
3. 在出现的详细信息飞出控件中，选择 **"操作"** 部分中的"编辑 **操作** "。
4. 在"**邮件操作**"部分，查看"垃圾邮件"、"高可信度垃圾邮件"、"网络钓鱼"和"高可信度网络钓鱼"裁定，以查看是否选择了以下任一值：  
   - **添加 X 标头**
   - **在主题行前添加文本**
   - **将邮件重定向到电子邮件地址**
   - **删除邮件**
   - **无操作**

   应用于所有客户 **的标准** 设置可能会Exchange Online Protection邮件。

有关详细信息，请参阅[在 EOP 中配置反垃圾邮件策略](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)。
