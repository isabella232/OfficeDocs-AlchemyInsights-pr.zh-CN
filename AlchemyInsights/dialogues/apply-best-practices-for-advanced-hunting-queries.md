---
title: 对高级搜寻查询应用最佳做法
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568476"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>应用高级搜寻查询的最佳实践

若要更快地获取结果并避免运行复杂查询时出现超时，请应用以下最佳实践：

- 在尝试新查询时，始终使用限制，以避免获取非常大的结果集。 此外， `count` 还用于对结果集大小进行初始评估。
- 首先使用时间筛选器。 理想情况下，将查询限制为七天。
- 在查询的开头，在时间筛选器之后，添加预计会删除大部分数据的筛选器。
- 在查找完整标记时，请使用 `has` 运算符，而不是 `contains` 。
- 对特定列而不是跨所有列运行搜索。
- 联接表时，首先指定行数较少的表。
- `project` 仅联接表中的必要列。

若要了解更多信息，请参阅 [高级搜寻查询最佳实践](https://go.microsoft.com/fwlink/?linkid=2144812)。
