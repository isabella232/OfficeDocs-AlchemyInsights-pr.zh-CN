---
title: 设备处于等待注册状态
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000657"
- "2508"
ms.openlocfilehash: 46bb390bd89d82bab8099f15f086746800cb4261
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800205"
---
# <a name="devices-are-in-awaiting-enrollment-state"></a>设备处于 "等待注册" 状态

桌面分析没有此设备的诊断数据。 

出现此问题的原因可能是您最近向目标集合中添加了设备, 但尚未发送数据。 这也意味着设备未与服务正常通信, 最新的诊断数据超过了28天。

请确保设备可以与服务通信。 有关详细信息, 请参阅 [终结点](https://docs.microsoft.com/sccm/desktop-analytics/enable-data-sharing#endpoints)。

有关 awainting 注册状态的详细信息, 请参阅[Monitor Connection Health](https://docs.microsoft.com/sccm/desktop-analytics/monitor-connection-health#awaiting-enrollment)。