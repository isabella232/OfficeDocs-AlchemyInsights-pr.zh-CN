---
title: SharePoint Online 限制
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931432"
---
# <a name="sharepoint-online-throttling"></a>SharePoint Online 限制

**重要说明**：许多 SharePoint Online 和 OneDrive 客户对在后台运行的服务运行关键业务应用程序。 其中包括内容迁移、数据丢失防护（DLP）和备份解决方案。 在这些前所未有的时间内，我们将采取措施，以确保在远程工作方案中，SharePoint Online 和 OneDrive 服务对依赖于该服务的用户保持高可用性和可靠性。

为支持此目标，我们已在工作日白天营业时对后台应用（迁移、DLP 和备份解决方案）实施了更严格的限制限制。 在这些情况中，您应认为这些应用程序的吞吐量非常有限。 但是，在夜间和周末的时间内，服务将准备好处理来自后台应用程序的较大数量的请求。

**SharePoint Online 限制**

SharePoint Online 使用限制来维护 SharePoint Online 服务的最佳性能和可靠性。 限制会限制用户操作或并发调用数量（通过脚本或代码），以防止资源的过度使用。 有关详细信息，请访问下面的链接。

- [避免在 SharePoint Online 中受限或遭屏蔽](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [数据迁移和 SPO 限制](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [SharePoint Online 和 OneDrive 迁移速度](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [使用指数回退处理 SharePoint Online 限制](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [容量规划和负载测试 SharePoint Online](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

