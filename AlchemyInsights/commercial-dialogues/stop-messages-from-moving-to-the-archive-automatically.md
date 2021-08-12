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
ms.openlocfilehash: df7443626308416e1d7edf4bc87c0eba95ec2c030d5ef3207513480873c1e3e7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929943"
---
# <a name="stop-messages-from-moving-to-the-archive-automatically"></a>自动阻止邮件移动到存档

如果使用保留策略，可以更改该策略中的保留时间以自动停止存档邮件。 操作步骤如下：

1. In the [Exchange admin center，](https://go.microsoft.com/fwlink/?linkid=2059104)choose **compliance management**  >  **retention tags**. 找到"移动到存档"保留标记。
2. 在保留标记中，将 (保留期) **更改为"** 从不"，以阻止保留策略自动存档项目。

> [!NOTE]
> 这将更改应用了此保留标记的所有邮箱的存档设置。
