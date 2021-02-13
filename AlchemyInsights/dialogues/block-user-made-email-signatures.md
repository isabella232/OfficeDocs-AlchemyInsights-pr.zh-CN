---
title: 阻止用户创建的电子邮件签名
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232696"
---
# <a name="block-user-made-email-signatures"></a>阻止用户创建的电子邮件签名

以下解决方案仅适用于在 Web 上的 Outlook 中创建的电子邮件签名。 只有在具有本地部署时，才能阻止 Outlook 应用中的Exchange Server。

1. 在管理中心中，选择 **"管理中心**  >  **Exchange"。**
2. 单击 **策略**  >  **Outlook Web App权限**。
3. 选择策略，然后单击铅笔图标进行编辑。
4. 单击 **功能**  >  **更多选项**。
5. 在 **"用户体验"** 下，清除"**电子邮件签名**"复选框，然后单击"保存 **"。**

**重要提示：** 如果在清除此复选框之前添加了签名，用户仍可以使用它。 要求他们删除它。
