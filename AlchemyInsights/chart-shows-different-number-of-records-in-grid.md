---
title: 图表显示网格中的不同记录数
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
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431363"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a>图表显示网格中的不同记录数

**症状**

对于仪表板页面上的图表，当你单击图表“...”，然后单击“查看记录”时，你将导航到网格页面以查看所有记录。有时，记录数会发生更改。

**原因**

这是因为原始仪表板页面上的图表与网格主页上的图表之间的视图不同。  

**解决方案**

1. 检查原始页面中的视图和网格中的视图，以查看它们是否不同。
2. 更改网格中的视图，以匹配原始页面中的视图。
3. 如果找不到正确的视图，通常意味着在应用设计器中未启用视图。
4. 转到特定应用的应用设计器，选择实体及其视图，查看要启用、保存、发布和关闭的视图。
5. 刷新页面。