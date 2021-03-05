---
title: 禁用网络扫描
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7b0f5c21a7e6afda0ee3000e75ee725cbadcedb7
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449047"
---
# <a name="disable-network-scan"></a>禁用网络扫描

网络共享扫描可能会影响性能。  若要确保客户端默认情况下不扫描网络共享/文件，请配置 Windows Defender应用程序中的以下 **设置：**

- DisableScanningMappedNetworkDrivesForFullScan
- DisableScanningNetworkFiles