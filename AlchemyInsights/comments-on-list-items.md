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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947478"
---
# <a name="comments-on-list-items"></a>对列表项的注释

用户将很快能够在列表项上添加和删除注释。 用户可以查看列表项上的所有注释，并在显示与项目相关的注释或活动的视图之间进行筛选。

**计时** ：

**目标版本** ：在2006年10月的中期逐步推出，并预期于11月中旬完成

**Standard release** ：在12月中旬前逐步推出并预期完成

**部署** ：针对整个组织的目标发布

在添加和删除注释之前，用户需要注意以下事项：

- 注释遵循 SharePoint 中的固有权限设置。
- 尚未构建以在新式用户界面中显示的经典列表（如任务列表）将不会有此注释功能。
- 对团队中的列表的注释在此版本中不可用。
- "搜索" 不会对注释编制索引。

通过在 **Set-spotenant** PowerShell cmdlet 中更改 **CommentsOnListItemsDisabled** 参数，管理员可以在组织级别禁用此功能。

当前不能禁用网站或列表级别的注释。 我们希望在后续更新中使用这些控件，可能在第一季度2021中。
