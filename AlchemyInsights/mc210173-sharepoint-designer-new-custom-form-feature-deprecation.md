---
title: MC210173 - SharePoint Designer 新自定义窗体功能弃用
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831796"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 - SharePoint Designer 新自定义窗体功能弃用

我们发现了一个会影响 SharePoint Online 中[创建自定义窗体](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2)的 SharePoint Designer 功能的问题。 仔细检查后，我们确定尚无此问题的解决方法，并已选择禁用自定义窗体创建功能，自 2020 年 4 月 25 日星期六 UTC 凌晨 3:00 起生效。 此更改不会影响在 SharePoint Online Designer 中编辑以前创建的窗体的能力或其他现有功能。

进行此更改后，用户在创建新窗体时可能收到错误：“无法将列表更改保存到服务器”。

以前曾利用 SharePoint Designer 创建自定义窗体的用户可以使用 [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) 来实现此目的。

PowerApps 是一款简单而强大的工具，它使用户可以在 SharePoint Online Modern 体验中操作，直接从浏览器窗口创建和编辑 SharePoint 列表和文档库的自定义窗体。 PowerApps 不需要传统编码知识或下载任何其他应用（如 InfoPath）。

**注意**：SharePoint Online Classic 用户需要暂时切换到 Modern 体验以便访问和使用 PowerApps；但是，SharePoint Online Classic 体验用户可以访问在 PowerApps 中创建的所有自定义窗体。
