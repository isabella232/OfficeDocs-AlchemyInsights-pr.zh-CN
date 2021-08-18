---
title: 配置隐私设置Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004632"
- "8367"
ms.openlocfilehash: 991f323249e15abd137c3e69b400e40503ed30dec6507cc5071a0b1af7f72bb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090288"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a>配置隐私设置Microsoft Edge

默认情况下，如果Microsoft Edge部署在非 Windows 平台，诊断数据和站点信息不会发送到 Microsoft。 但是，Microsoft Edge部署在Windows 10，诊断数据和站点信息根据用户的诊断数据Windows[发送](https://go.microsoft.com/fwlink/?linkid=2132472)。

若要配置Microsoft Edge组织处理数据收集的方式，请使用以下组策略：
- [MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) 可打开使用情况和故障相关数据的报告。
- [SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470)发送用于改进网站Microsoft 服务。

若要了解更多信息，请参阅 [配置策略设置](https://go.microsoft.com/fwlink/?linkid=2132577)。
