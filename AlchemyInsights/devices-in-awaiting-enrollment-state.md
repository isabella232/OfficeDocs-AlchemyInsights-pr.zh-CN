---
title: 设备正在等待注册状态
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000657"
- "2508"
ms.openlocfilehash: 068e6dc7fae7221add027d335854b708ccc963532fda53be9d8f54bc578abab6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031036"
---
# <a name="devices-are-in-awaiting-enrollment-state"></a>设备的状态为"等待注册"

桌面分析没有此设备的诊断数据。 

This issue may occur because you recently added the device to the target collection and it hasn't sent data. 它还意味着设备未与服务正确通信，并且最新的诊断数据超过 28 天。

确保设备可以与服务通信。 有关详细信息，请参阅 [终结点](https://docs.microsoft.com/configmgr/desktop-analytics/enable-data-sharing#endpoints)。

有关等待注册状态的信息，请参阅 [监视连接运行状况](https://docs.microsoft.com/configmgr/desktop-analytics/monitor-connection-health#awaiting-enrollment)。