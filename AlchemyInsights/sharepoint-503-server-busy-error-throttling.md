---
title: SharePoint Online 限制
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: b157ce22962ac1616d6e9b3a5475edaec7fed9f7
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34761249"
---
# <a name="sharepoint-online-throttling"></a>SharePoint Online 限制

尝试导航到 SharePoint 或 OneDrive 网站时, 用户可能会收到 "503 服务器占线" 错误。 

此错误可能是由 SharePoint 服务中的限制导致的。 SharePoint Online 使用限制来维护 SharePoint Online 服务的最佳性能和可靠性。 限制会限制用户操作或并发调用数量（通过脚本或代码），以防止资源的过度使用。 如果您被限制，99% 都是因为自定义代码。

有关限制的详细信息, 请参阅[避免在 SharePoint Online 中受到限制或被阻止](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)。

如果您认为此错误与限制无关, 可以通过导航到[消息中心](https://portal.office.com/adminportal/home#/MessageCenter)来检查租户上是否有活动的维护正在发生。

 最后, 请确保访问 "[服务运行状况](https://portal.office.com/adminportal/home#/servicehealth)" 页, 以检查可能发生的任何咨询/事件。
