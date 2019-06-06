---
title: 127访问电子邮件时是否收到 TenantAccessBlockedException 错误？
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: 5613138e7613deb264a7ab2c966f8b9c4a24763d
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736393"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>在尝试使用 SharePoint 或 OneDrive 时, 维护邮件为只读

当尝试使用 SharePoint 或 OneDrive 时, 用户可能会收到一个只读的维护消息。

通过导航到 "[消息中心](https://portal.office.com/adminportal/home#/MessageCenter)" 检查租户上是否有活动的维护正在发生。 最后, 请确保访问 "[服务运行状况](https://portal.office.com/adminportal/home#/servicehealth)" 页, 以检查可能发生的任何咨询/事件。

如果消息中心或服务运行状况仪表板均未对租户的当前维护内容进行任何说明, 则这可能是浏览器缓存问题。

请先尝试清除浏览器缓存, 然后再导航到该网站。

- 在 Microsoft Edge 浏览器中, 转到 "更多设置"

- 在 "清除浏览" 下, 选择 "选择要清除的内容"。
- 选中 "Cookie 和保存的网站数据" 复选框, 然后选择 "清除"。

**注意**: 使用其他浏览器 (如 Firefox 或 Chrome) 时, 这些步骤可能会有所不同。

