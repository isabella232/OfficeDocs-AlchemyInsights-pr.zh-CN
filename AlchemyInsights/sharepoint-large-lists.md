---
title: SharePoint大型列表
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: c67632e323f2068faba06779b94ba4fd8e9f319e18cefb7977bd3038ca770210
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53941557"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>在网站中处理大型列表和SharePoint

SharePoint列表和库可以包含多达 3000 万个项目，但是当它们具有的项目超过 5，000 个时，当您尝试使用列表视图阈值时，您可能会看到"列表视图阈值"错误。 此阈值是为了维持服务的性能。 不能更改。 若要避免达到此阈值：

**使用新式**

显示许多项的视图在新式体验中效果最佳。 [使用新式体验](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) 以避免在经典体验中可能看到的错误。

**添加索引**

按没有索引的列进行筛选或排序时，可能会看到错误消息。 [从"列表"](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0)菜单手动添加 **设置，** 再从"索引列"**添加** 索引。

**编辑列表视图**

如果在使用大型列表时发生错误， [请编辑列表视图](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)。

以下四项更改将删除列表视图阈值错误。 进行所有四项更改以删除所有错误。 如果仍收到错误，请查看管理 [大型列表和库](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)。

1. Select **None** from both **First sort by the column** and Then sort by the **column**.
2. Select **None** from both **First group by the column** and Then group by the **column**.
3. 为 **"** 总计"部分的所有 **列选择"无** "。
4. 从"列"部分取消选择除一列外的所有 **列** 进行显示。

