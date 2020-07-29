---
title: 删除 Teams 专用频道
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431359"
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