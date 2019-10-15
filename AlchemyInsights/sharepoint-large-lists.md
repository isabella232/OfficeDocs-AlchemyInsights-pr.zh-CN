---
title: SharePoint 大型列表
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 2/12/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 222ad554de0d94dcfd4e34e9a2c6aa8ab4e6f81f
ms.sourcegitcommit: d7e1b097d3866782f508527c797426dc56c6ba17
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2019
ms.locfileid: "37488507"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="0950e-102">在 SharePoint 中处理大型列表和库</span><span class="sxs-lookup"><span data-stu-id="0950e-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="0950e-103">SharePoint 列表和库最多可包含30000000个项目，但当它们的项目数超过5000时，您可能会在尝试使用它们时看到列表视图阈值错误。</span><span class="sxs-lookup"><span data-stu-id="0950e-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="0950e-104">此阈值已生效，可维护服务的性能。</span><span class="sxs-lookup"><span data-stu-id="0950e-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="0950e-105">无法更改。</span><span class="sxs-lookup"><span data-stu-id="0950e-105">It can't be changed.</span></span> <span data-ttu-id="0950e-106">若要避免出现此阈值，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="0950e-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="0950e-107">**使用新式**</span><span class="sxs-lookup"><span data-stu-id="0950e-107">**Use modern**</span></span>

<span data-ttu-id="0950e-108">显示许多项目最适用于新式体验的视图。</span><span class="sxs-lookup"><span data-stu-id="0950e-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="0950e-109">[使用新式体验](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9)避免在经典体验中可能会看到的错误。</span><span class="sxs-lookup"><span data-stu-id="0950e-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="0950e-110">**添加索引**</span><span class="sxs-lookup"><span data-stu-id="0950e-110">**Add indexes**</span></span>

<span data-ttu-id="0950e-111">当按不包含索引的列进行筛选或排序时，您可能会看到一条错误消息。</span><span class="sxs-lookup"><span data-stu-id="0950e-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="0950e-112">从 "设置" 菜单中的 "**列表设置**" 手动[添加索引](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0)，然后添加索引**列**。</span><span class="sxs-lookup"><span data-stu-id="0950e-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="0950e-113">**编辑列表视图**</span><span class="sxs-lookup"><span data-stu-id="0950e-113">**Edit the list view**</span></span>

<span data-ttu-id="0950e-114">如果在使用大型列表时出现错误，请[编辑列表视图](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)。</span><span class="sxs-lookup"><span data-stu-id="0950e-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="0950e-115">下面的四个更改将删除列表视图阈值错误。</span><span class="sxs-lookup"><span data-stu-id="0950e-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="0950e-116">做出全部四个更改以删除所有错误。</span><span class="sxs-lookup"><span data-stu-id="0950e-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="0950e-117">如果仍收到错误，请检查 "[管理大型列表和库](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)"。</span><span class="sxs-lookup"><span data-stu-id="0950e-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="0950e-118">从**第一个排序**中选择 "**无**"，**再按列进行排序**。</span><span class="sxs-lookup"><span data-stu-id="0950e-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="0950e-119">从**第一个 group 的列**中选择 "**无**"，**然后按列进行分组**。</span><span class="sxs-lookup"><span data-stu-id="0950e-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="0950e-120">对 "**总计**" 部分中的所有列选择 "**无**"。</span><span class="sxs-lookup"><span data-stu-id="0950e-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="0950e-121">取消选择除一列之外的所有列以显示从 "**列**" 部分。</span><span class="sxs-lookup"><span data-stu-id="0950e-121">Deselect all but one column for display from the **Columns** section.</span></span>

