---
title: 应用高级搜寻查询的最佳实践
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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930123"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>应用高级搜寻查询的最佳实践

若要更快地获取结果并避免在运行复杂查询时出现超时，请应用以下最佳实践：

- 尝试新查询时，请始终使用限制，以避免获得非常大的结果集。 此外，使用 对应用程序结果集 `count` 进行初始评估。
- 首先使用时间筛选器。 理想情况下，将查询限制为七天。
- 在查询的开头，在时间筛选器之后，添加预计会删除大部分数据的筛选器。
- 在查找完整令牌时，请使用 `has` 运算符，而不是 `contains` 。
- 对特定列而不是跨所有列运行搜索。
- 联接表时，首先指定行数较少的表。
- `project` 仅联接表中的必要列。

若要了解更多信息，请参阅 [高级搜寻查询最佳实践](https://go.microsoft.com/fwlink/?linkid=2144812)。
