---
title: Microsoft Edge配置隐私设置
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003843"
- "6892"
ms.openlocfilehash: 24721325aefd4a8c0dbeb7864ce6da637c4df932694d4b6fff80cab5bb5b4319
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54114162"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge配置隐私设置

默认情况下，如果Microsoft Edge部署在非Windows平台，诊断数据和站点信息不会发送给 Microsoft。 但是，Microsoft Edge部署在Windows 10，诊断数据和站点信息根据用户的诊断数据Windows[发送](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)。

若要配置Microsoft Edge组织处理数据收集的方式，请使用以下组策略：
- [MetricsReportingEnabled：](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled)此策略允许报告使用情况和故障相关的数据。
- [SendSiteInfoToImproveServices：](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices)此策略发送用于改进网站Microsoft 服务。

若要了解更多信息，请参阅 [配置策略设置](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)。