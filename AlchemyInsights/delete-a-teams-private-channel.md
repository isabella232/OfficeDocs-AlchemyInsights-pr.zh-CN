---
title: 删除 Teams 专用频道
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730905"
---
# <a name="delete-a-teams-private-channel"></a>删除 Teams 专用频道

Microsoft 注意到，如果为基础 SharePoint 网站启用了 SharePoint 保留策略，则删除 Teams 专用频道时会遇到问题。 Microsoft 正在着手解决这一问题。 在此期间，可以使用以下解决方法删除专用频道。

**从 Sharepoint 保留策略中排除团队/网站集。**

1. 转到 Office 365 管理门户，然后在左侧导航窗格中选择“**全部显示**”。
2. 在**管理中心**下，转到“**安全与合规**” > “**数据丢失防护**” > “**策略**”。
3. 确定适用于 SharePoint 网站的任何策略，并修改策略，以便包含专用频道的团队的 SharePoint 网站不包含在保留策略中。
4. 保存策略。
    策略设置可能需要长达 24 小时才能生效。
    排除网站后，可删除专用频道。  
    
你***也许***能够通过在 Android 设备上使用 Microsoft Teams 删除专用频道。 

有关 SharePoint 的相关信息，请参阅[无法删除 SharePoint Online 或 OneDrive for Business 中的项目](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)。