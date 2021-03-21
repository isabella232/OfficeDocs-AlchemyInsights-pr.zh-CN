---
title: 通过使用数据目录变量而不是硬编码路径来修改 Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897427"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>通过使用数据目录变量而不是硬编码路径来修改 Microsoft Edge

例如，在 Windows 上，要将配置文件数据存储在用户的本地应用程序数据下而不是默认位置下，请将 *UserDataDir* 策略设置为 **${local_app_data}\Edge\Profile**。

有关详细信息，请参阅[创建 Microsoft Edge 用户数据目录变量](https://docs.microsoft.com/deployedge/microsoft-edge-policies)。