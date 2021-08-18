---
title: 使用Microsoft Edge变量（而不是硬编码路径）修改数据库
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
ms.openlocfilehash: 235696d17711726da57d9a09c23b5b13140a28d7645299ef120a4b2c7b395c5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54113406"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>使用Microsoft Edge变量（而不是硬编码路径）修改数据库

例如，在 Windows 上，要将配置文件数据存储在用户的本地应用程序数据下而不是默认位置下，请将 **UserDataDir** 策略设置为 **${local_app_data}\Edge\Profile**。 

若要了解更多信息，请参阅[Create Microsoft Edge user data directory variables](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars)。