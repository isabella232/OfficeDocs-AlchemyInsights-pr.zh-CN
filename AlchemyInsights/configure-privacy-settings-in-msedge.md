---
title: 在 Microsoft Edge 中配置隐私设置
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
ms.openlocfilehash: 2367a7a55d1837fa7c7095fd0ac10ff1cf7ae72d
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403789"
---
# <a name="configure-privacy-settings-in-microsoft-edge"></a><span data-ttu-id="ee3f3-102">在 Microsoft Edge 中配置隐私设置</span><span class="sxs-lookup"><span data-stu-id="ee3f3-102">Configure privacy settings in Microsoft Edge</span></span>

<span data-ttu-id="ee3f3-103">默认情况下，如果 Microsoft Edge 部署在非 Windows 平台上，诊断数据和站点信息不会发送到 Microsoft。</span><span class="sxs-lookup"><span data-stu-id="ee3f3-103">By default, if Microsoft Edge is deployed on non-Windows platforms, diagnostic data and site information aren't sent to Microsoft.</span></span> <span data-ttu-id="ee3f3-104">但是，如果 Microsoft Edge 部署在 Windows 10 上，诊断数据和站点信息根据用户的 [Windows 诊断数据设置发送](https://go.microsoft.com/fwlink/?linkid=2132472)。</span><span class="sxs-lookup"><span data-stu-id="ee3f3-104">However, if Microsoft Edge is deployed on Windows 10, diagnostic data and site information are sent according to users' [Windows Diagnostic data settings](https://go.microsoft.com/fwlink/?linkid=2132472).</span></span>

<span data-ttu-id="ee3f3-105">若要配置 Microsoft Edge 如何处理组织的数据收集，请使用以下组策略：</span><span class="sxs-lookup"><span data-stu-id="ee3f3-105">To configure how Microsoft Edge handles data collection for your organization, use the following group policies:</span></span>
- <span data-ttu-id="ee3f3-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) 可打开使用情况和故障相关数据的报告。</span><span class="sxs-lookup"><span data-stu-id="ee3f3-106">[MetricsReportingEnabled](https://go.microsoft.com/fwlink/?linkid=2132470) turns on reporting of usage and crash-related data.</span></span>
- <span data-ttu-id="ee3f3-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) 发送用于改进 Microsoft 服务的网站信息。</span><span class="sxs-lookup"><span data-stu-id="ee3f3-107">[SendSiteInfoToImproveServices](https://go.microsoft.com/fwlink/?linkid=2132470) sends site information used to improve Microsoft services.</span></span>

<span data-ttu-id="ee3f3-108">若要了解更多信息，请参阅 [配置策略设置](https://go.microsoft.com/fwlink/?linkid=2132577)。</span><span class="sxs-lookup"><span data-stu-id="ee3f3-108">To learn more, see [Configure policy settings](https://go.microsoft.com/fwlink/?linkid=2132577).</span></span>
