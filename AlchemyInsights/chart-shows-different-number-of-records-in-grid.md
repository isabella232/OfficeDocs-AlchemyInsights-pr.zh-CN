---
title: 图表显示网格中的不同记录数
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
- "5611"
- "9002930"
ms.openlocfilehash: e499a439e7cf7e9ecbb6566f9f089f3b7b82f48e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47793748"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="e0363-102">图表显示网格中的不同记录数</span><span class="sxs-lookup"><span data-stu-id="e0363-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="e0363-103">**症状**</span><span class="sxs-lookup"><span data-stu-id="e0363-103">**Symptom**</span></span>

<span data-ttu-id="e0363-104">对于仪表板页面上的图表，当你单击图表“...”，然后单击“查看记录”时，你将导航到网格页面以查看所有记录。有时，记录数会发生更改。</span><span class="sxs-lookup"><span data-stu-id="e0363-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="e0363-105">**原因**</span><span class="sxs-lookup"><span data-stu-id="e0363-105">**Cause**</span></span>

<span data-ttu-id="e0363-106">这是因为原始仪表板页面上的图表与网格主页上的图表之间的视图不同。</span><span class="sxs-lookup"><span data-stu-id="e0363-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="e0363-107">**解决方案**</span><span class="sxs-lookup"><span data-stu-id="e0363-107">**Solution**</span></span>

1. <span data-ttu-id="e0363-108">检查原始页面中的视图和网格中的视图，以查看它们是否不同。</span><span class="sxs-lookup"><span data-stu-id="e0363-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="e0363-109">更改网格中的视图，以匹配原始页面中的视图。</span><span class="sxs-lookup"><span data-stu-id="e0363-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="e0363-110">如果找不到正确的视图，通常意味着在应用设计器中未启用视图。</span><span class="sxs-lookup"><span data-stu-id="e0363-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="e0363-111">转到特定应用的应用设计器，选择实体及其视图，查看要启用、保存、发布和关闭的视图。</span><span class="sxs-lookup"><span data-stu-id="e0363-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="e0363-112">刷新页面。</span><span class="sxs-lookup"><span data-stu-id="e0363-112">Refresh the page.</span></span>