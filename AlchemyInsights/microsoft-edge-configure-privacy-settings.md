---
title: Microsoft Edge 配置隐私设置
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
ms.openlocfilehash: dcd1d91dcde1f585caf0e1e3af30946513a0f26c
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599458"
---
# <a name="microsoft-edge-configure-privacy-settings"></a>Microsoft Edge 配置隐私设置

默认情况下，如果 Microsoft Edge 部署在非 Windows 平台上，则不会将诊断数据和网站信息发送给 Microsoft。 但是，如果 Microsoft Edge 部署在 Windows 10 上，诊断数据和网站信息将根据用户的 [Windows 诊断数据设置](https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization)发送。

若要配置 Microsoft Edge 处理组织数据收集的方式，请使用以下组策略：
- [MetricsReportingEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#metricsreportingenabled)：此策略允许报告使用情况和与崩溃相关的数据。
- [SendSiteInfoToImproveServices](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#sendsiteinfotoimproveservices)：此策略发送用于改进 Microsoft 服务的网站信息。

若要了解详细信息，请参阅 [配置策略设置](https://docs.microsoft.com/deployedge/microsoft-edge-enterprise-privacy-settings#configure-policy-settings)。