---
title: 在尝试使用 SharePoint 或 OneDrive 时, 维护邮件为只读
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 5b1e56253d6deeb0f9ba2f753eff5c00ff9c51a2
ms.sourcegitcommit: cd79ecca88b2cb166f78f44ab8bc4e8136729418
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/23/2019
ms.locfileid: "36620713"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>在尝试使用 SharePoint 或 OneDrive 时, 维护邮件为只读

当尝试将 SharePoint 或 OneDrive 用于下列方案之一时, 用户可能会收到**只读的维护**消息。 

-   计划的或活动的维护活动。  通过导航到[邮件中心](https://portal.office.com/adminportal/home#/messagecenter)来检查它们。
-   可能发生的高优先级活动服务事件。 通过导航到 "[服务运行状况](https://portal.office.com/adminportal/home#/servicehealth)" 检查是否有任何咨询/事件。
-   一种很小的自动修复恢复方案, 由于可能持续30分钟以上的服务器上的任何意外事件而发生。 
    
    这些次要恢复没有邮件中心或服务运行状况帖子, 但您应尽快恢复正常。

在极少数情况下, 我们发现上面列出的三个方案中的一种原因是原因, 服务已还原, 但尚未清除用户浏览器缓存。

请先尝试清除浏览器缓存, 然后再导航到该网站。

1. 在 Microsoft Edge 浏览器中, 选择 "**设置**", 然后选择 "**隐私和安全**"。
2. 在 "**清除浏览**" 下, 选择 "**选择要清除的内容**"。
3. 选择 " **cookie" 和 "保存的网站数据**", 然后选择 "**清除**"。

>[!Note] 
> 这些步骤在使用其他浏览器 (如 Mozilla Firefox 或 Google Chrome) 时可能有所不同。

>[!Note] 
> 另一种方法是在新的 InPrivate 窗口中打开 SharePoint 网站或 OneDrive。