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
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403733"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="de82f-102">工作流未启动</span><span class="sxs-lookup"><span data-stu-id="de82f-102">Workflow is not starting</span></span>

- <span data-ttu-id="de82f-103">SharePoint 2010 和 SharePoint 2013 工作流未启动。</span><span class="sxs-lookup"><span data-stu-id="de82f-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="de82f-104">如果工作流未启动，则可能会遇到临时服务问题，用户可能会遇到工作流进度的间歇性延迟。</span><span class="sxs-lookup"><span data-stu-id="de82f-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="de82f-105">检查 [服务运行状况仪表板](https://admin.microsoft.com/AdminPortal/Home/servicehealth) 以查看您的组织是否受到影响。</span><span class="sxs-lookup"><span data-stu-id="de82f-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="de82f-106">如果自你第一次看到此问题以来超过 24 小时，请记录支持票证。</span><span class="sxs-lookup"><span data-stu-id="de82f-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="de82f-107">在许多情况下，我们已经在研究解决方案。</span><span class="sxs-lookup"><span data-stu-id="de82f-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="de82f-108">请给我们至少 24 小时才能完成解决方案。</span><span class="sxs-lookup"><span data-stu-id="de82f-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="de82f-109">SharePoint 2010 工作流在开始时延迟。</span><span class="sxs-lookup"><span data-stu-id="de82f-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="de82f-110">如果以大批量方式触发工作流，则会出现此情况。</span><span class="sxs-lookup"><span data-stu-id="de82f-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="de82f-111"> (，例如，当一次添加多个项目时) 。</span><span class="sxs-lookup"><span data-stu-id="de82f-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="de82f-112">工作流不是设计为实时运行，因此延迟是按设计行为。</span><span class="sxs-lookup"><span data-stu-id="de82f-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="de82f-113">如果工作流是 XMOL 中复杂的可扩展对象标记 (语言) ，则编译速度可能很慢。</span><span class="sxs-lookup"><span data-stu-id="de82f-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="de82f-114">查看 [本文](https://support.microsoft.com//kb/3043697) 。</span><span class="sxs-lookup"><span data-stu-id="de82f-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="de82f-115">您应该使用 Microsoft SharePoint 2013 工作流平台类型简化或重新设计工作流。</span><span class="sxs-lookup"><span data-stu-id="de82f-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="de82f-116">如果您的工作流历史记录已变得很大，您可能需要清除项目或创建新的历史记录列表。</span><span class="sxs-lookup"><span data-stu-id="de82f-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="de82f-117">详细信息： [清除工作流历史记录](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="de82f-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="de82f-118">相关主题</span><span class="sxs-lookup"><span data-stu-id="de82f-118">Related topics</span></span>
<span data-ttu-id="de82f-119">想要尝试 SharePoint Online 中的 Microsoft Flow？</span><span class="sxs-lookup"><span data-stu-id="de82f-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="de82f-120">创建流</span><span class="sxs-lookup"><span data-stu-id="de82f-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="de82f-121">SharePoint 和流</span><span class="sxs-lookup"><span data-stu-id="de82f-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
