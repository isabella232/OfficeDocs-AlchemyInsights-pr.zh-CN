---
title: 性能问题-SharePoint或OneDrive
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
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911832"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint或OneDrive用户速度慢、无法访问或不可用

SharePoint或OneDrive速度较慢、无法访问或不可用，或者显示服务不可用或 503 错误，原因如下：
  
- 如果您的 SharePoint 或 OneDrive 网站对于多个用户是缓慢或延迟的，则可能会遇到临时服务问题，即用户在访问网站或内容时遇到间歇性延迟SharePoint导航OneDrive错误。 请查看[服务运行状况仪表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)，了解你的组织是否受到影响。
  
- 用户尝试导航到其他站点或访问网站时，SharePoint *503* 服务器OneDrive错误。 此错误可能是由服务中的限制SharePoint导致的。 SharePoint Online 使用限制来维护 SharePoint Online 服务的最佳性能和可靠性。 限制（通过脚本或代码）对用户操作数量或并发性调用进行限制，以阻止资源的过度使用。 有关限制详细信息，请参阅避免在 SharePoint [Online 中受限制或被阻止](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)。

- 如果你在使用经典或新式网站或页面 **时** SharePoint性能，则使用 [页面](https://aka.ms/perftool)诊断工具分析页面。 
  
- 如果你仍然遇到常规性能缓慢的问题，请查看本文底部的资源：针对[SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)的性能调整简介
  