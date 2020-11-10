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
# <a name="comments-on-list-items"></a><span data-ttu-id="0c46b-102">对列表项的注释</span><span class="sxs-lookup"><span data-stu-id="0c46b-102">Comments on List items</span></span>

<span data-ttu-id="0c46b-103">用户将很快能够在列表项上添加和删除注释。</span><span class="sxs-lookup"><span data-stu-id="0c46b-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="0c46b-104">用户可以查看列表项上的所有注释，并在显示与项目相关的注释或活动的视图之间进行筛选。</span><span class="sxs-lookup"><span data-stu-id="0c46b-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="0c46b-105">**计时** ：</span><span class="sxs-lookup"><span data-stu-id="0c46b-105">**Timing** :</span></span>

<span data-ttu-id="0c46b-106">**目标版本** ：在2006年10月的中期逐步推出，并预期于11月中旬完成</span><span class="sxs-lookup"><span data-stu-id="0c46b-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="0c46b-107">**Standard release** ：在12月中旬前逐步推出并预期完成</span><span class="sxs-lookup"><span data-stu-id="0c46b-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="0c46b-108">**部署** ：针对整个组织的目标发布</span><span class="sxs-lookup"><span data-stu-id="0c46b-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="0c46b-109">在添加和删除注释之前，用户需要注意以下事项：</span><span class="sxs-lookup"><span data-stu-id="0c46b-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="0c46b-110">注释遵循 SharePoint 中的固有权限设置。</span><span class="sxs-lookup"><span data-stu-id="0c46b-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="0c46b-111">尚未构建以在新式用户界面中显示的经典列表（如任务列表）将不会有此注释功能。</span><span class="sxs-lookup"><span data-stu-id="0c46b-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="0c46b-112">对团队中的列表的注释在此版本中不可用。</span><span class="sxs-lookup"><span data-stu-id="0c46b-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="0c46b-113">"搜索" 不会对注释编制索引。</span><span class="sxs-lookup"><span data-stu-id="0c46b-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="0c46b-114">通过在 **Set-spotenant** PowerShell cmdlet 中更改 **CommentsOnListItemsDisabled** 参数，管理员可以在组织级别禁用此功能。</span><span class="sxs-lookup"><span data-stu-id="0c46b-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="0c46b-115">当前不能禁用网站或列表级别的注释。</span><span class="sxs-lookup"><span data-stu-id="0c46b-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="0c46b-116">我们希望在后续更新中使用这些控件，可能在第一季度2021中。</span><span class="sxs-lookup"><span data-stu-id="0c46b-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
