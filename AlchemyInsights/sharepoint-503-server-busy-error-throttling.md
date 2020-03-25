---
title: SharePoint Online 限制
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931216"
---
# <a name="sharepoint-online-throttling"></a>SharePoint Online 限制

**重要说明**：许多 SharePoint Online 和 OneDrive 客户对在后台运行的服务运行关键业务应用程序。 其中包括内容迁移、数据丢失防护（DLP）和备份解决方案。 在这些前所未有的时间内，我们将采取措施，以确保在远程工作方案中，SharePoint Online 和 OneDrive 服务对依赖于该服务的用户保持高可用性和可靠性。

为支持此目标，我们已在工作日白天营业时对后台应用（迁移、DLP 和备份解决方案）实施了更严格的限制限制。 在这些情况中，您应认为这些应用程序的吞吐量非常有限。 但是，在夜间和周末的时间内，服务将准备好处理来自后台应用程序的较大数量的请求。

**503服务器忙碌错误**

尝试导航到 SharePoint 或 OneDrive 网站时，用户可能会收到 "503 服务器占线" 错误。 

此错误可能是由 SharePoint 服务中的限制导致的。 SharePoint Online 使用限制来维护 SharePoint Online 服务的最佳性能和可靠性。 限制会限制用户操作或并发调用数量（通过脚本或代码），以防止资源的过度使用。 

有关限制的详细信息，请参阅[避免在 SharePoint Online 中受到限制或被阻止](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)。

如果您认为此错误与限制无关，可以通过导航到[消息中心](https://portal.office.com/adminportal/home#/MessageCenter)来检查租户上是否有活动的维护正在发生。

 最后，请确保访问 "[服务运行状况](https://portal.office.com/adminportal/home#/servicehealth)" 页，以检查可能发生的任何咨询/事件。

