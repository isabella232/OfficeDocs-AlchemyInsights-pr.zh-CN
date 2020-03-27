---
title: 通用迁移性能指南
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932469"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="f12a5-102">通用迁移性能指南</span><span class="sxs-lookup"><span data-stu-id="f12a5-102">General migration performance guidance</span></span>

<span data-ttu-id="f12a5-103">**重要说明**：许多 SharePoint Online 和 OneDrive 客户针对后台运行的服务来运行业务关键应用程序。</span><span class="sxs-lookup"><span data-stu-id="f12a5-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f12a5-104">其中包括内容迁移、数据丢失防护 (DLP) 和备份解决方案。</span><span class="sxs-lookup"><span data-stu-id="f12a5-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f12a5-105">在这个前所未有的时代，我们正在采取行动，以确保 SharePoint Online 和 OneDrive 服务保持高可用性和可靠性，为在远程工作场景中比以往任何时候都更依赖这些服务的用户提供便利。</span><span class="sxs-lookup"><span data-stu-id="f12a5-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f12a5-106">为了支持这一目标，我们对在工作日日间时间段内运行的后台应用（迁移、DLP 和备份解决方案）实施了更严格的限制。</span><span class="sxs-lookup"><span data-stu-id="f12a5-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f12a5-107">预计这些应用应该会在这段时间内实现非常有限的吞吐量。</span><span class="sxs-lookup"><span data-stu-id="f12a5-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f12a5-108">不过，在相应区域的夜间和周末时间段内，服务将可以处理来自后台应用的大量请求。</span><span class="sxs-lookup"><span data-stu-id="f12a5-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f12a5-109">**迁移性能指南**</span><span class="sxs-lookup"><span data-stu-id="f12a5-109">**Migration performance guidance**</span></span>

<span data-ttu-id="f12a5-p103">迁移性能受网络基础结构、文件大小、迁移时间和限制的影响。了解这些有助于你规划和最大化迁移效率。</span><span class="sxs-lookup"><span data-stu-id="f12a5-p103">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling. Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="f12a5-112">通用迁移性能指南</span><span class="sxs-lookup"><span data-stu-id="f12a5-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
