---
title: 工作流未启动
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794757"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="307a0-102">工作流未启动</span><span class="sxs-lookup"><span data-stu-id="307a0-102">Workflow is not starting</span></span>

- <span data-ttu-id="307a0-103">SharePoint 2010 和 SharePoint 2013 工作流未启动。</span><span class="sxs-lookup"><span data-stu-id="307a0-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="307a0-104">如果工作流未启动，则可能存在临时服务问题，用户可能会遇到工作流进度间歇延迟的问题。</span><span class="sxs-lookup"><span data-stu-id="307a0-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="307a0-105">检查 [服务运行状况仪表板](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) 以查看您的组织是否受到影响。</span><span class="sxs-lookup"><span data-stu-id="307a0-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="307a0-106">如果在你首次看到此问题后过去已经超过24小时，请记录一个支持票证。</span><span class="sxs-lookup"><span data-stu-id="307a0-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="307a0-107">在许多情况下，我们已经在研究解决方案。</span><span class="sxs-lookup"><span data-stu-id="307a0-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="307a0-108">请至少为我们提供24小时的时间来完成解决方案。</span><span class="sxs-lookup"><span data-stu-id="307a0-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="307a0-109">SharePoint 2010 工作流在启动时延迟。</span><span class="sxs-lookup"><span data-stu-id="307a0-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="307a0-110">如果在大型批处理中触发工作流，则会发生此情况。</span><span class="sxs-lookup"><span data-stu-id="307a0-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="307a0-111"> (例如，如果一次添加了多个项目) 。</span><span class="sxs-lookup"><span data-stu-id="307a0-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="307a0-112">工作流设计为实时运行，因此延迟是设计行为。</span><span class="sxs-lookup"><span data-stu-id="307a0-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="307a0-113">如果工作流是复杂的可扩展对象标记语言 (XMOL) ，则编译可能会很慢。</span><span class="sxs-lookup"><span data-stu-id="307a0-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="307a0-114">请[查看本文。](https://support.microsoft.com//kb/3043697)</span><span class="sxs-lookup"><span data-stu-id="307a0-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="307a0-115">应简化工作流或使用 Microsoft SharePoint 2013 工作流平台类型对其进行重新设计。</span><span class="sxs-lookup"><span data-stu-id="307a0-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="307a0-116">如果您的工作流历史记录增长很大，您可能需要清除这些项或创建一个新的历史记录列表。</span><span class="sxs-lookup"><span data-stu-id="307a0-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="307a0-117">详细信息： [清除工作流历史记录](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="307a0-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="307a0-118">相关主题</span><span class="sxs-lookup"><span data-stu-id="307a0-118">Related topics</span></span>
<span data-ttu-id="307a0-119">想要在 SharePoint Online 中试用 Microsoft 流吗？</span><span class="sxs-lookup"><span data-stu-id="307a0-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="307a0-120">创建流</span><span class="sxs-lookup"><span data-stu-id="307a0-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="307a0-121">SharePoint 和流</span><span class="sxs-lookup"><span data-stu-id="307a0-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


