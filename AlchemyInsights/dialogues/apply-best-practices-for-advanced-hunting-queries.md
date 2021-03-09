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
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="bf4ea-102">应用高级搜寻查询的最佳实践</span><span class="sxs-lookup"><span data-stu-id="bf4ea-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="bf4ea-103">若要更快地获取结果并避免运行复杂查询时出现超时，请应用以下最佳实践：</span><span class="sxs-lookup"><span data-stu-id="bf4ea-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="bf4ea-104">在尝试新查询时，始终使用限制，以避免获取非常大的结果集。</span><span class="sxs-lookup"><span data-stu-id="bf4ea-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="bf4ea-105">此外， `count` 还用于对结果集大小进行初始评估。</span><span class="sxs-lookup"><span data-stu-id="bf4ea-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="bf4ea-106">首先使用时间筛选器。</span><span class="sxs-lookup"><span data-stu-id="bf4ea-106">Use time filters first.</span></span> <span data-ttu-id="bf4ea-107">理想情况下，将查询限制为七天。</span><span class="sxs-lookup"><span data-stu-id="bf4ea-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="bf4ea-108">在查询的开头，在时间筛选器之后，添加预计会删除大部分数据的筛选器。</span><span class="sxs-lookup"><span data-stu-id="bf4ea-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="bf4ea-109">在查找完整标记时，请使用 `has` 运算符，而不是 `contains` 。</span><span class="sxs-lookup"><span data-stu-id="bf4ea-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="bf4ea-110">对特定列而不是跨所有列运行搜索。</span><span class="sxs-lookup"><span data-stu-id="bf4ea-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="bf4ea-111">联接表时，首先指定行数较少的表。</span><span class="sxs-lookup"><span data-stu-id="bf4ea-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="bf4ea-112">`project` 仅联接表中的必要列。</span><span class="sxs-lookup"><span data-stu-id="bf4ea-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="bf4ea-113">若要了解更多信息，请参阅 [高级搜寻查询最佳实践](https://go.microsoft.com/fwlink/?linkid=2144812)。</span><span class="sxs-lookup"><span data-stu-id="bf4ea-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
