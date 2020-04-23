---
title: SharePoint 大型列表
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767275"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>在 SharePoint 中处理大型列表和库

SharePoint 列表和库最多可包含30000000个项目，但当它们的项目数超过5000时，您可能会在尝试使用它们时看到列表视图阈值错误。 此阈值是为了维持服务的性能。 不能更改。 若要避免出现此阈值，请执行以下操作：

**使用新式**

显示许多项目最适用于新式体验的视图。 [使用新式体验](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9)避免在经典体验中可能会看到的错误。

**添加索引**

当按不包含索引的列进行筛选或排序时，您可能会看到一条错误消息。 从 "设置" 菜单中的 "**列表设置**" 手动[添加索引](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0)，然后添加索引**列**。

**编辑列表视图**

如果在使用大型列表时出现错误，请[编辑列表视图](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)。

下面的四个更改将删除列表视图阈值错误。 做出全部四个更改以删除所有错误。 如果仍收到错误，请检查 "[管理大型列表和库](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)"。

1. 从**第一个排序**中选择 "**无**"，**再按列进行排序**。
2. 从**第一个 group 的列**中选择 "**无**"，**然后按列进行分组**。
3. 对 "**总计**" 部分中的所有列选择 "**无**"。
4. 取消选择除一列之外的所有列以显示从 "**列**" 部分。

