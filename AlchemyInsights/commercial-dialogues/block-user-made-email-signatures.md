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
ms.openlocfilehash: ad743cea4b8735b35b90bd5bf3d0b5b933184ed82858e828a68beb2ca2f8270c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54103542"
---
# <a name="block-user-made-email-signatures"></a>阻止用户创建的电子邮件签名

以下解决方案仅适用于在 Outlook 网页版 中创建的电子邮件签名。 如果你拥有本地部署Outlook，你只能阻止 Exchange Server。

1. 在管理中心中，选择"管理 **中心**  >  **Exchange"。**
2. 单击 **"权限**  >  **Outlook Web App策略"。**
3. 选择策略，然后单击铅笔图标进行编辑。
4. 单击 **"功能**  >  **""更多选项"。**
5. 在 **"用户体验"** 下，清除"**电子邮件签名**"复选框，然后单击"保存 **"。**

**重要提示：** 如果在清除此复选框之前添加了签名，则用户仍可以使用它。 要求他们将其删除。
