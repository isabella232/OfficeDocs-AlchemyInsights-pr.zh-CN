---
title: 自动阻止邮件移动到存档
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
- "3100008"
- "7217"
ms.openlocfilehash: 2cb3e29dfd4f422e946b7887d4d44f373ff03794
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735673"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a>自动阻止邮件移动到存档

如果使用保留策略，可以更改该策略中的保留时间以自动停止存档邮件。 操作步骤如下：

1. 在 [Exchange 管理中心中，](https://go.microsoft.com/fwlink/?linkid=2059104)选择 **"合规性管理**  >  **""保留标记"。** 找到"移动到存档"保留标记。
2. 在保留标记中，将 (保留期) **更改为"** 从不"，以阻止保留策略自动存档项目。

> [!NOTE]
> 这将更改应用了此保留标记的所有邮箱的存档设置。
