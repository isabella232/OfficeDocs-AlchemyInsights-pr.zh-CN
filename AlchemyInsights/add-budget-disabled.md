---
title: 为什么我禁用了"添加预算"按钮？
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822625"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a><span data-ttu-id="f5325-102">为什么我禁用了"添加预算"按钮？</span><span class="sxs-lookup"><span data-stu-id="f5325-102">Why is the Add budget button disabled for me?</span></span>

<span data-ttu-id="f5325-103">若要创建预算，您需要以下权限之一：</span><span class="sxs-lookup"><span data-stu-id="f5325-103">To create a budget, you need one of the following permissions:</span></span>

- <span data-ttu-id="f5325-104">管理组、订阅、资源组作用域</span><span class="sxs-lookup"><span data-stu-id="f5325-104">Management Group, Subscription, Resource Group Scopes</span></span>
- <span data-ttu-id="f5325-105">成本管理参与者</span><span class="sxs-lookup"><span data-stu-id="f5325-105">Cost Management Contributor</span></span>
- <span data-ttu-id="f5325-106">所有者</span><span class="sxs-lookup"><span data-stu-id="f5325-106">Owner</span></span>
- <span data-ttu-id="f5325-107">参与者</span><span class="sxs-lookup"><span data-stu-id="f5325-107">Contributor</span></span>
- <span data-ttu-id="f5325-108">仅企业客户：注册、部门、帐户作用域</span><span class="sxs-lookup"><span data-stu-id="f5325-108">Enterprise Customer Only: Enrollment, Department, Account Scopes</span></span>
- <span data-ttu-id="f5325-109">注册管理员 (注册范围设置) </span><span class="sxs-lookup"><span data-stu-id="f5325-109">Enrollment Admin (set budget at Enrollment scope)</span></span>
- <span data-ttu-id="f5325-110">部门管理员 (部门范围内设置) </span><span class="sxs-lookup"><span data-stu-id="f5325-110">Department Admin (set budget at Department scope)</span></span>
- <span data-ttu-id="f5325-111">帐户所有者 (作用域设置预算) </span><span class="sxs-lookup"><span data-stu-id="f5325-111">Account Owner (set budget at Account scope)</span></span>
- <span data-ttu-id="f5325-112">仅新式客户协议：计费帐户、计费配置文件、发票部分范围</span><span class="sxs-lookup"><span data-stu-id="f5325-112">Modern Customer Agreement Only: Billing Account, Billing Profile, Invoice Section Scopes</span></span>
- <span data-ttu-id="f5325-113">Azure 订阅创建者</span><span class="sxs-lookup"><span data-stu-id="f5325-113">Azure subscription creator</span></span>

<span data-ttu-id="f5325-114">**当当当月的成本已超预算时，我创建了一个预算。为什么我没有收到警报？**</span><span class="sxs-lookup"><span data-stu-id="f5325-114">**I created a budget when my cost for the current month was already over-budget. Why did I not receive an alert?**</span></span>  
<span data-ttu-id="f5325-115">如果在创建预算时已超出给定成本阈值，将不会触发警报。</span><span class="sxs-lookup"><span data-stu-id="f5325-115">If you have already exceeded a given cost threshold when you create a budget that alert will not fire.</span></span> <span data-ttu-id="f5325-116">新周期开始后，如果超出阈值，将触发警报。</span><span class="sxs-lookup"><span data-stu-id="f5325-116">Once a new cycle begins, if you breach the threshold then the alert will fire.</span></span>

<span data-ttu-id="f5325-117">**当超过定义的一个预算警报阈值后，我应何时收到警报？**</span><span class="sxs-lookup"><span data-stu-id="f5325-117">**When should I expect to receive an alert after I exceed one of my defined budget alert thresholds?**</span></span>  
<span data-ttu-id="f5325-118">每 4 小时评估一次预算。</span><span class="sxs-lookup"><span data-stu-id="f5325-118">Budgets are evaluated every 4 hours.</span></span> <span data-ttu-id="f5325-119">使用数据到达预算系统至少需要 8 小时。</span><span class="sxs-lookup"><span data-stu-id="f5325-119">It takes a minimum of 8 hours for usage data to reach the budgets system.</span></span> <span data-ttu-id="f5325-120">考虑到这一点，超过阈值后，警报可能需要 12 小时才能触发。</span><span class="sxs-lookup"><span data-stu-id="f5325-120">Given this, alerts may take as long as 12 hours to fire after you exceed a threshold.</span></span>

<span data-ttu-id="f5325-121">**Why is the Start date button disabled when I select a Month or Billing month reset period？**</span><span class="sxs-lookup"><span data-stu-id="f5325-121">**Why is the Start date button disabled when I select a Month or Billing month reset period?**</span></span>  
<span data-ttu-id="f5325-122">预算与当前日历月或当前计费周期 (（如果选择了"计费月份") ）。</span><span class="sxs-lookup"><span data-stu-id="f5325-122">Budgets are aligned to the current calendar month or current billing period (in the case where Billing Month is selected).</span></span> <span data-ttu-id="f5325-123">因此，我们将预先填充此值。</span><span class="sxs-lookup"><span data-stu-id="f5325-123">Therefore, we pre-populate this value for you.</span></span>

<span data-ttu-id="f5325-124">**为什么我在预算创建体验中看不到我成本的图形？**</span><span class="sxs-lookup"><span data-stu-id="f5325-124">**Why do I not see a graph of my costs in the budget creation experience?**</span></span>  
<span data-ttu-id="f5325-125">我们至少需要 2 个月的成本数据，然后才能呈现图形来帮助你创建预算。</span><span class="sxs-lookup"><span data-stu-id="f5325-125">We need a minimum of 2 months of cost data before we can render a graph to assist you with budget creation.</span></span>

<span data-ttu-id="f5325-126">**为什么我无法针对刚创建的订阅设置预算？**</span><span class="sxs-lookup"><span data-stu-id="f5325-126">**Why can't I set a budget against a subscription I just created?**</span></span>  
<span data-ttu-id="f5325-127">创建订阅后，在针对数据设置预算之前，需要 24-48 小时处理数据。</span><span class="sxs-lookup"><span data-stu-id="f5325-127">After the creation of a subscription, the data takes 24-48 hours to process before setting a budget against it.</span></span>

<span data-ttu-id="f5325-128">**预算 API 资源**</span><span class="sxs-lookup"><span data-stu-id="f5325-128">**Budget API Resources**</span></span>

- <span data-ttu-id="f5325-129">[预算 API v1：](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)提供用于创建和更新预算的操作。</span><span class="sxs-lookup"><span data-stu-id="f5325-129">[Budgets API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to create and update budgets.</span></span> <span data-ttu-id="f5325-130">使用预算 API，可以设置预算阈值，并配置多个警报以在接近该阈值时触发。</span><span class="sxs-lookup"><span data-stu-id="f5325-130">Using the Budgets API, you can set a budget threshold and configure multiple alerts to fire as you approach that threshold.</span></span> <span data-ttu-id="f5325-131">警报可以触发电子邮件或 Azure 操作组以执行自动化。</span><span class="sxs-lookup"><span data-stu-id="f5325-131">Alerts can trigger an email or an Azure Action Group to perform automation.</span></span> <span data-ttu-id="f5325-132">注意：此 API 筛选与查询 API 筛选/维度不一致。</span><span class="sxs-lookup"><span data-stu-id="f5325-132">Note: Filtering for this API does not align with Query API filtering / dimensions.</span></span>
- <span data-ttu-id="f5325-133">[预算 API v2：](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)使用比 v1 更高的成本筛选功能创建预算。</span><span class="sxs-lookup"><span data-stu-id="f5325-133">[Budgets API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Create budgets with greater cost filtering capabilities than v1.</span></span> <span data-ttu-id="f5325-134">筛选与查询和维度 API 中使用的协定一致。</span><span class="sxs-lookup"><span data-stu-id="f5325-134">Filtering aligns to the contract used in our Query and Dimensions APIs.</span></span> <span data-ttu-id="f5325-135">这是建议用于今后使用的预算 API。</span><span class="sxs-lookup"><span data-stu-id="f5325-135">This is the recommended budgets API to use moving forward.</span></span>
- <span data-ttu-id="f5325-136">[Dimensions](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)：提供用于获取各种范围内使用情况支持的维度的操作。</span><span class="sxs-lookup"><span data-stu-id="f5325-136">[Dimensions](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to get supported dimensions for your usage under a variety of scopes.</span></span> <span data-ttu-id="f5325-137">使用 Dimensions API，您可以检索维度列表，这些维度可用作使用查询 API 生成查询的输入。</span><span class="sxs-lookup"><span data-stu-id="f5325-137">Using the Dimensions API, you can retrieve a list of dimensions that can be used as inputs for generating queries with the Query API.</span></span>
- <span data-ttu-id="f5325-138">[查询](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)：提供基于您提供的查询获取聚合成本和使用率数据的操作。</span><span class="sxs-lookup"><span data-stu-id="f5325-138">[Query](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to get aggregated cost and usage data based on the query you supply.</span></span> <span data-ttu-id="f5325-139">使用查询 API，可以在所有可用维度上指定所需的筛选、排序和分组 (可从 Dimensions API) 。</span><span class="sxs-lookup"><span data-stu-id="f5325-139">Using the Query API, you can specify your desired filtering, sorting and grouping on all available dimensions (which are accessed from the Dimensions API).</span></span>

<span data-ttu-id="f5325-140">**预测成本**</span><span class="sxs-lookup"><span data-stu-id="f5325-140">**Forecasted Costs**</span></span>

<span data-ttu-id="f5325-141">**为什么我在成本分析中看不到成本预测？**</span><span class="sxs-lookup"><span data-stu-id="f5325-141">**Why don’t I see forecasts for my costs in Cost Analysis?**</span></span>  
<span data-ttu-id="f5325-142">成本分析中可能缺少预测预测的原因有多种，其中一些原因如下：</span><span class="sxs-lookup"><span data-stu-id="f5325-142">There are multiple reasons why the forecast projection might be missing for you in Cost Analysis, some of them are as follows:</span></span>

1. <span data-ttu-id="f5325-143">如果成本数据少于 10 天，将不会加载预测图表。</span><span class="sxs-lookup"><span data-stu-id="f5325-143">If your cost data is less than 10 days old, the forecast chart will not load.</span></span> <span data-ttu-id="f5325-144">该模型需要至少 10 天的最近成本数据，以用于准确的预测</span><span class="sxs-lookup"><span data-stu-id="f5325-144">The model requires at least 10 days of recent cost data for accurate projections</span></span>
2. <span data-ttu-id="f5325-145">如果选择了历史日期，则预测图表将不可见。</span><span class="sxs-lookup"><span data-stu-id="f5325-145">If you have selected historic dates, then the forecast chart will not be visible.</span></span> <span data-ttu-id="f5325-146">Please select a date range with future dates for the forecast chart to be displayed</span><span class="sxs-lookup"><span data-stu-id="f5325-146">Please select a date range with future dates for the forecast chart to be displayed</span></span>
3. <span data-ttu-id="f5325-147">如果你的帐户具有多种货币，预测图表将仅针对"所有成本以美元为单位"的项目成本</span><span class="sxs-lookup"><span data-stu-id="f5325-147">If your account has multiple currencies, the forecast chart will only project costs for 'All costs in USD'</span></span>

<span data-ttu-id="f5325-148">**为什么我对资源进行更改时预测没有变化？**</span><span class="sxs-lookup"><span data-stu-id="f5325-148">**Why doesn’t the forecast change when I make changes to my resources?**</span></span>  
<span data-ttu-id="f5325-149">预测模型需要几天的时间来考虑帐户中的更改，并且不会根据资源更改立即进行预测</span><span class="sxs-lookup"><span data-stu-id="f5325-149">The forecast model requires a couple of days to account for changes in the account and does not make immediate projections based on change in resources</span></span>  
<span data-ttu-id="f5325-150">对于资源增加或减少的较大步骤，模型需要更长的调整时间以适应这些更改，以考虑异常</span><span class="sxs-lookup"><span data-stu-id="f5325-150">For larger steps of increase or decrease in resources, the model will take slightly longer to adjust to these changes to account for anomalies</span></span>

<span data-ttu-id="f5325-151">**为什么我在预订或市场购买后预测会增加？**</span><span class="sxs-lookup"><span data-stu-id="f5325-151">**Why does my forecast increase after I make a reservation or Marketplace purchase?**</span></span>  
<span data-ttu-id="f5325-152">预测模型会考虑你的"实际成本"，并不单独考虑使用情况和购买。对于一次购买，该模型将在 10 天后减少预测，以说明成本的突然增加</span><span class="sxs-lookup"><span data-stu-id="f5325-152">The forecast model considers your 'Actual Cost' and does not account for usage and purchase separately.For a one-time purchase, the model will decrease the projections after 10 days to account for the sudden increase in costs</span></span>

<span data-ttu-id="f5325-153">**我想查看单个维度预测，例如 (预测。指示器)**</span><span class="sxs-lookup"><span data-stu-id="f5325-153">**I want to see forecasts for a single dimension (eg. Meter)**</span></span>  
<span data-ttu-id="f5325-154">预测当前支持总成本预测，而非单米预测。</span><span class="sxs-lookup"><span data-stu-id="f5325-154">Forecast currently supports total cost projections and not for individual meters.</span></span> <span data-ttu-id="f5325-155">因此，当"分组者"一个维度时，投影将为维度中所有项的总计</span><span class="sxs-lookup"><span data-stu-id="f5325-155">Hence, when 'Grouped by' a dimension, the projections will be for total of all items in the dimension</span></span>

<span data-ttu-id="f5325-156">**推荐文档**</span><span class="sxs-lookup"><span data-stu-id="f5325-156">**Recommended Documents**</span></span>

- [<span data-ttu-id="f5325-157">什么是 Azure 成本管理？</span><span class="sxs-lookup"><span data-stu-id="f5325-157">What is Azure Cost Management?</span></span>](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="f5325-158">Azure 成本管理最佳做法</span><span class="sxs-lookup"><span data-stu-id="f5325-158">Azure Cost Management best practices</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="f5325-159">分析成本和费用</span><span class="sxs-lookup"><span data-stu-id="f5325-159">Analyze your costs and spending</span></span>](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="f5325-160">使用成本分析探索和分析成本</span><span class="sxs-lookup"><span data-stu-id="f5325-160">Explore and analyze costs with Cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="f5325-161">Azure 成本管理：定价</span><span class="sxs-lookup"><span data-stu-id="f5325-161">Azure Cost Management: Pricing</span></span>](https://azure.microsoft.com/services/cost-management/#pricing)
- [<span data-ttu-id="f5325-162">查看成本分析中的成本</span><span class="sxs-lookup"><span data-stu-id="f5325-162">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [<span data-ttu-id="f5325-163">视频教程：在 Azure 门户创建预算</span><span class="sxs-lookup"><span data-stu-id="f5325-163">Video tutorial: Create a budget in the Azure portal</span></span>](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [<span data-ttu-id="f5325-164">查看和自定义预算的先决条件</span><span class="sxs-lookup"><span data-stu-id="f5325-164">Prerequisites for viewing and customizing budgets</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [<span data-ttu-id="f5325-165">创建和管理预算</span><span class="sxs-lookup"><span data-stu-id="f5325-165">Create and manage budgets</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [<span data-ttu-id="f5325-166">使用 Azure 操作组和预算 API 配置自动化</span><span class="sxs-lookup"><span data-stu-id="f5325-166">Configure automation with Azure Action Groups and Budgets API</span></span>](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [<span data-ttu-id="f5325-167">使用成本警报监视使用情况和费用</span><span class="sxs-lookup"><span data-stu-id="f5325-167">Use cost alerts to monitor usage and spending</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="f5325-168">成本管理最佳做法</span><span class="sxs-lookup"><span data-stu-id="f5325-168">Cost Management best practices</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

<span data-ttu-id="f5325-169">**教程视频**</span><span class="sxs-lookup"><span data-stu-id="f5325-169">**Tutorial videos**</span></span>

- [<span data-ttu-id="f5325-170">在 Azure 门户创建预算</span><span class="sxs-lookup"><span data-stu-id="f5325-170">Create a budget in the Azure portal</span></span>](https://go.microsoft.com/fwlink/?linkid=2146761)
- [<span data-ttu-id="f5325-171">使用预算 API 和操作组管理成本</span><span class="sxs-lookup"><span data-stu-id="f5325-171">Manage costs with the Budgets API and Action Groups</span></span>](https://go.microsoft.com/fwlink/?linkid=2147038)