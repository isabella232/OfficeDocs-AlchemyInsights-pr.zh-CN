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
ms.openlocfilehash: a083ac548d818f0ed922a6d17b38c3a3df2d86c0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58333337"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a>自动阻止邮件移动到存档

如果使用保留策略，可以更改该策略中的保留时间以自动停止存档邮件。 操作步骤如下：

1. In the [Exchange admin center，](https://go.microsoft.com/fwlink/?linkid=2059104)choose **compliance management**  >  **retention tags**. 找到"移动到存档"保留标记。
2. 在保留标记中，将"存档 **(") "从不** "，以阻止保留策略自动存档项目。

**注意**：这将更改应用了此保留标记的所有邮箱的存档设置。
