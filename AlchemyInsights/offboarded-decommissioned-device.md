---
title: 从设备清单中删除已载或已停用设备的问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 814301e9cd8197e62dcca68ab3bdde1618d210f73a744b53bb5af7b861eb02bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54076633"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>从设备清单中删除已载或已停用设备的问题

Microsoft Defender for Endpoint 当前不允许从设备清单中手动删除载出或停用的设备的设备记录。

出于安全目的，设备作为历史记录在门户中保留最多 180 天。 但是，设备数据将按照配置的保留期进行清除。

**注意：** 载出或停用的设备会在七天后自动 **切换到** 非活动状态。 此外，过去 30 天内未处于活动状态的设备不会纳入反映你的组织曝光分数危险和漏洞管理 Microsoft 安全分数的数据中。
 
如果仍不想在"设备清单"视图中看到某些设备，请尝试放置设备标记以从"设备清单"视图中筛选出停用的设备。

有关详细信息，请参阅：

[从 Microsoft Defender for Endpoint 服务载出设备](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[曝光分数（以危险和漏洞管理](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[修复 Microsoft Defender for Endpoint 中的不正常传感器](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[如何在第 1 部分 (标记) ](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[如何在第 2 部分 (标记) ](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[如何在第 3 部分 (标记) ](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




