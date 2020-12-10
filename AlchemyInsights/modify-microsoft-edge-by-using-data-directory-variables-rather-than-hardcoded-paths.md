---
title: 使用数据目录变量而不是硬编码路径修改 Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608819"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>使用数据目录变量而不是硬编码路径修改 Microsoft Edge

例如，在 Windows 上，若要将配置文件数据存储在用户的本地应用程序数据（而不是默认位置）下，请将 **UserDataDir** 策略设置为 **$ {local_app_data} \Edge\Profile**。 

若要了解详细信息，请参阅 [Create Microsoft Edge user data directory 变量](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars)。