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
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255151"
---
# <a name="enable-device"></a>启用设备

**使用 Powershell 命令启用设备**

运行以下命令：

- 若要获取设备对象， `Get-MsolDevice -Name <Name>`
- 若要启用设备， `Enable-MsolDevice -DeviceId <DeviceId>`

有关在托管域上配置混合加入的信息，请参阅["配置混合加入"。](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)
