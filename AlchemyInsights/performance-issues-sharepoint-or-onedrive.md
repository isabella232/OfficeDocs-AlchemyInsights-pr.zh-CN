---
title: 性能问题-SharePoint 或 OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771891"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint 或 OneDrive 速度慢、不可访问或对多个用户不可用

SharePoint 或 OneDrive 的速度可能很慢、不可访问或不可用，或者因以下几个原因而显示服务不可用或503错误：
  
- 如果您的 SharePoint 或 OneDrive 网站的多个用户的速度较慢或延迟，则在访问 SharePoint 网站或 OneDrive 内容时，用户可能会遇到间歇延迟或导航错误的临时服务问题。 请查看[服务运行状况仪表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)，了解你的组织是否受到影响。
  
- 尝试导航到 SharePoint 或 OneDrive 网站时，用户可能会收到 " *503 服务器占线* " 错误。 此错误可能是由 SharePoint 服务中的限制导致的。 SharePoint Online 使用限制来维护 SharePoint Online 服务的最佳性能和可靠性。 限制（通过脚本或代码）对用户操作数量或并发性调用进行限制，以阻止资源的过度使用。 有关限制的详细信息，请参阅 [避免在 SharePoint Online 中受到限制或被阻止](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)。

- 如果您在使用 **经典** 或 **新式** SharePoint 网站或页面时遇到性能降低的情况，请使用 [页面诊断工具](https://aka.ms/perftool) 来分析页面。
  
- 如果仍遇到常规低性能，请查看本文底部的资源： [SharePoint Online 的性能优化简介](https://go.microsoft.com/fwlink/?linkid=2024334)
  