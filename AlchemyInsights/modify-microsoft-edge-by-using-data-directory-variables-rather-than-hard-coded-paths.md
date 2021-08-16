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
ms.openlocfilehash: e3ad930ec79ef82f3bf95e84cb88e8bb9aea13637d8e59d845b486604664b137
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53992281"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>通过使用数据目录变量而不是硬编码路径来修改 Microsoft Edge

例如，在 Windows 上，要将配置文件数据存储在用户的本地应用程序数据下而不是默认位置下，请将 *UserDataDir* 策略设置为 **${local_app_data}\Edge\Profile**。

有关详细信息，请参阅[创建 Microsoft Edge 用户数据目录变量](https://docs.microsoft.com/deployedge/microsoft-edge-policies)。