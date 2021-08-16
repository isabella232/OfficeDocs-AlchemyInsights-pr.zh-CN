---
title: 启用设备
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 4722ccf6847fc6c02616dbc62d59a2a87c089f77ae79c0a916211af6c5f2a6d0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003462"
---
# <a name="enable-device"></a>启用设备

**使用 Powershell 命令启用设备**

运行以下命令：

- 若要获取 device 对象： `Get-MsolDevice -Name <Name>`
- 若要启用设备： `Enable-MsolDevice -DeviceId <DeviceId>`

有关在托管域上配置混合加入的信息，请参阅 [配置混合加入](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)。
