---
title: 对列表项的注释
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724144"
---
# <a name="comments-on-list-items"></a>对列表项的注释

用户可以查看列表项上的所有注释，并筛选显示与项目相关的注释或活动的视图。

用户需要先注意以下事项，然后才能添加和删除注释：

- 注释遵循 SharePoint 中固有的权限设置。
- 尚未构建以在新式用户界面（如任务列表）中显示经典列表将没有此注释功能。
- 此版本对 Teams 中的列表进行评论不可用。
- 搜索不会对注释编制索引。

管理员可以在组织级别禁用此功能，方法为更改 **Set-SPOTenant** PowerShell cmdlet 中的 **CommentsOnListItemsDisabled** 参数。

当前无法禁用站点或列表级别的注释。 我们希望在稍后的更新（可能在 2021 年第一季度）中提供这些控件。
