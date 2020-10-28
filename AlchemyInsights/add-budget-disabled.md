---
title: 为什么 "添加预算" 按钮对我是禁用的？
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6464"
ms.openlocfilehash: 18edad73f617ba180cb08576ee6e5fa8faf07128
ms.sourcegitcommit: 9a7b85eae0bb775bc2498a83d8f5fedb72a6451e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/27/2020
ms.locfileid: "48769586"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a><span data-ttu-id="9ded3-102">为什么 "添加预算" 按钮对我是禁用的？</span><span class="sxs-lookup"><span data-stu-id="9ded3-102">Why is the Add budget button disabled for me?</span></span>

<span data-ttu-id="9ded3-103">若要创建预算，您需要以下权限之一：</span><span class="sxs-lookup"><span data-stu-id="9ded3-103">To create a budget, you need one of the following permissions:</span></span>

- <span data-ttu-id="9ded3-104">管理组、订阅、资源组作用域</span><span class="sxs-lookup"><span data-stu-id="9ded3-104">Management Group, Subscription, Resource Group Scopes</span></span>
- <span data-ttu-id="9ded3-105">成本管理参与者</span><span class="sxs-lookup"><span data-stu-id="9ded3-105">Cost Management Contributor</span></span>
- <span data-ttu-id="9ded3-106">所有者</span><span class="sxs-lookup"><span data-stu-id="9ded3-106">Owner</span></span>
- <span data-ttu-id="9ded3-107">参与者</span><span class="sxs-lookup"><span data-stu-id="9ded3-107">Contributor</span></span>
- <span data-ttu-id="9ded3-108">仅企业客户：注册、部门、帐户范围</span><span class="sxs-lookup"><span data-stu-id="9ded3-108">Enterprise Customer Only: Enrollment, Department, Account Scopes</span></span>
- <span data-ttu-id="9ded3-109">注册管理员 (在注册作用域设置预算) </span><span class="sxs-lookup"><span data-stu-id="9ded3-109">Enrollment Admin (set budget at Enrollment scope)</span></span>
- <span data-ttu-id="9ded3-110">部门管理员 (设置部门范围内的预算) </span><span class="sxs-lookup"><span data-stu-id="9ded3-110">Department Admin (set budget at Department scope)</span></span>
- <span data-ttu-id="9ded3-111">帐户所有者 (设置 "帐户" 范围内的预算) </span><span class="sxs-lookup"><span data-stu-id="9ded3-111">Account Owner (set budget at Account scope)</span></span>
- <span data-ttu-id="9ded3-112">仅限新式客户协议：帐单帐户、帐单配置文件、发票部分范围</span><span class="sxs-lookup"><span data-stu-id="9ded3-112">Modern Customer Agreement Only: Billing Account, Billing Profile, Invoice Section Scopes</span></span>
- <span data-ttu-id="9ded3-113">Azure 订阅创建程序</span><span class="sxs-lookup"><span data-stu-id="9ded3-113">Azure subscription creator</span></span>

<span data-ttu-id="9ded3-114">**当我的当前月成本已过预算时，我创建了预算。为什么我没有收到通知？**</span><span class="sxs-lookup"><span data-stu-id="9ded3-114">**I created a budget when my cost for the current month was already over-budget. Why did I not receive an alert?**</span></span>  
<span data-ttu-id="9ded3-115">如果您在创建预算时已超出给定的成本阈值，则不会触发预警。</span><span class="sxs-lookup"><span data-stu-id="9ded3-115">If you have already exceeded a given cost threshold when you create a budget that alert will not fire.</span></span> <span data-ttu-id="9ded3-116">新周期开始后，如果您违反阈值，则会触发警报。</span><span class="sxs-lookup"><span data-stu-id="9ded3-116">Once a new cycle begins, if you breach the threshold then the alert will fire.</span></span>

<span data-ttu-id="9ded3-117">**我在超过我定义的某个预算警报阈值后何时应该收到通知？**</span><span class="sxs-lookup"><span data-stu-id="9ded3-117">**When should I expect to receive an alert after I exceed one of my defined budget alert thresholds?**</span></span>  
<span data-ttu-id="9ded3-118">每4小时对预算进行一次评估。</span><span class="sxs-lookup"><span data-stu-id="9ded3-118">Budgets are evaluated every 4 hours.</span></span> <span data-ttu-id="9ded3-119">使用率数据最少需要8小时才能到达预算系统。</span><span class="sxs-lookup"><span data-stu-id="9ded3-119">It takes a minimum of 8 hours for usage data to reach the budgets system.</span></span> <span data-ttu-id="9ded3-120">在此情况下，在超过阈值后触发警报可能需要等待12个小时。</span><span class="sxs-lookup"><span data-stu-id="9ded3-120">Given this, alerts may take as long as 12 hours to fire after you exceed a threshold.</span></span>

<span data-ttu-id="9ded3-121">**为什么在我选择一个月或帐单重置时段时禁用开始日期按钮？**</span><span class="sxs-lookup"><span data-stu-id="9ded3-121">**Why is the Start date button disabled when I select a Month or Billing month reset period?**</span></span>  
<span data-ttu-id="9ded3-122">预算与当前的日历月或当前帐单期对齐 (在) 中选择计费月的情况下。</span><span class="sxs-lookup"><span data-stu-id="9ded3-122">Budgets are aligned to the current calendar month or current billing period (in the case where Billing Month is selected).</span></span> <span data-ttu-id="9ded3-123">因此，我们为你预填充此值。</span><span class="sxs-lookup"><span data-stu-id="9ded3-123">Therefore, we pre-populate this value for you.</span></span>

<span data-ttu-id="9ded3-124">**为什么我在预算创建体验中看不到我的成本关系图？**</span><span class="sxs-lookup"><span data-stu-id="9ded3-124">**Why do I not see a graph of my costs in the budget creation experience?**</span></span>  
<span data-ttu-id="9ded3-125">我们至少需要2个月的成本数据，才能呈现可帮助您创建预算的图形。</span><span class="sxs-lookup"><span data-stu-id="9ded3-125">We need a minimum of 2 months of cost data before we can render a graph to assist you with budget creation.</span></span>

<span data-ttu-id="9ded3-126">**为什么我无法针对刚刚创建的订阅设置预算？**</span><span class="sxs-lookup"><span data-stu-id="9ded3-126">**Why can't I set a budget against a subscription I just created?**</span></span>  
<span data-ttu-id="9ded3-127">创建订阅后，在为数据设置预算之前，数据需要24-48 小时才能处理。</span><span class="sxs-lookup"><span data-stu-id="9ded3-127">After the creation of a subscription, the data takes 24-48 hours to process before setting a budget against it.</span></span>

<span data-ttu-id="9ded3-128">**预算 API 资源**</span><span class="sxs-lookup"><span data-stu-id="9ded3-128">**Budget API Resources**</span></span>

- <span data-ttu-id="9ded3-129">[预算 API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)：提供用于创建和更新预算的操作。</span><span class="sxs-lookup"><span data-stu-id="9ded3-129">[Budgets API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to create and update budgets.</span></span> <span data-ttu-id="9ded3-130">使用预算 API，您可以设置预算阈值，并配置多个警报以在您接近该阈值时触发。</span><span class="sxs-lookup"><span data-stu-id="9ded3-130">Using the Budgets API, you can set a budget threshold and configure multiple alerts to fire as you approach that threshold.</span></span> <span data-ttu-id="9ded3-131">警报可触发电子邮件或 Azure 操作组以执行自动化。</span><span class="sxs-lookup"><span data-stu-id="9ded3-131">Alerts can trigger an email or an Azure Action Group to perform automation.</span></span> <span data-ttu-id="9ded3-132">注意：此 API 的筛选不与查询 API 筛选/维度相一致。</span><span class="sxs-lookup"><span data-stu-id="9ded3-132">Note: Filtering for this API does not align with Query API filtering / dimensions.</span></span>
- <span data-ttu-id="9ded3-133">[预算 API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)：使用高于 v1 的成本筛选功能创建预算。</span><span class="sxs-lookup"><span data-stu-id="9ded3-133">[Budgets API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Create budgets with greater cost filtering capabilities than v1.</span></span> <span data-ttu-id="9ded3-134">筛选与我们的查询和维度 Api 中使用的约定相适应。</span><span class="sxs-lookup"><span data-stu-id="9ded3-134">Filtering aligns to the contract used in our Query and Dimensions APIs.</span></span> <span data-ttu-id="9ded3-135">这是建议的预算 API，以供将来使用。</span><span class="sxs-lookup"><span data-stu-id="9ded3-135">This is the recommended budgets API to use moving forward.</span></span>
- <span data-ttu-id="9ded3-136">[维度](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)：提供在各种范围内为您的使用获取受支持的维度的操作。</span><span class="sxs-lookup"><span data-stu-id="9ded3-136">[Dimensions](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to get supported dimensions for your usage under a variety of scopes.</span></span> <span data-ttu-id="9ded3-137">使用维度 API，您可以检索可用作在查询 API 中生成查询的输入的维度列表。</span><span class="sxs-lookup"><span data-stu-id="9ded3-137">Using the Dimensions API, you can retrieve a list of dimensions that can be used as inputs for generating queries with the Query API.</span></span>
- <span data-ttu-id="9ded3-138">[查询](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)：提供根据您提供的查询来获取聚合成本和使用情况数据的操作。</span><span class="sxs-lookup"><span data-stu-id="9ded3-138">[Query](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to get aggregated cost and usage data based on the query you supply.</span></span> <span data-ttu-id="9ded3-139">使用查询 API，您可以指定所需的筛选，在所有可用维度上进行排序和分组， (可从维度 API) 访问。</span><span class="sxs-lookup"><span data-stu-id="9ded3-139">Using the Query API, you can specify your desired filtering, sorting and grouping on all available dimensions (which are accessed from the Dimensions API).</span></span>

<span data-ttu-id="9ded3-140">**预测成本**</span><span class="sxs-lookup"><span data-stu-id="9ded3-140">**Forecasted Costs**</span></span>

<span data-ttu-id="9ded3-141">**为什么我在成本分析中看不到我对成本的预测？**</span><span class="sxs-lookup"><span data-stu-id="9ded3-141">**Why don’t I see forecasts for my costs in Cost Analysis?**</span></span>  
<span data-ttu-id="9ded3-142">在成本分析中可能缺少预测计划的多个原因，其中一些原因如下：</span><span class="sxs-lookup"><span data-stu-id="9ded3-142">There are multiple reasons why the forecast projection might be missing for you in Cost Analysis, some of them are as follows:</span></span>

1. <span data-ttu-id="9ded3-143">如果您的成本数据少于10天，则不会加载预测图表。</span><span class="sxs-lookup"><span data-stu-id="9ded3-143">If your cost data is less than 10 days old, the forecast chart will not load.</span></span> <span data-ttu-id="9ded3-144">模型需要至少10天的最近成本数据才能实现准确的预测</span><span class="sxs-lookup"><span data-stu-id="9ded3-144">The model requires at least 10 days of recent cost data for accurate projections</span></span>
2. <span data-ttu-id="9ded3-145">如果您已选择历史日期，则预测图表将不可见。</span><span class="sxs-lookup"><span data-stu-id="9ded3-145">If you have selected historic dates, then the forecast chart will not be visible.</span></span> <span data-ttu-id="9ded3-146">请选择要显示的预测图表的日期范围和未来日期</span><span class="sxs-lookup"><span data-stu-id="9ded3-146">Please select a date range with future dates for the forecast chart to be displayed</span></span>
3. <span data-ttu-id="9ded3-147">如果你的帐户有多种货币，则预测图表将仅对 "所有费用都是 USD" 的成本进行项目</span><span class="sxs-lookup"><span data-stu-id="9ded3-147">If your account has multiple currencies, the forecast chart will only project costs for 'All costs in USD'</span></span>

<span data-ttu-id="9ded3-148">**为什么在我对我的资源进行更改时预测不会发生变化？**</span><span class="sxs-lookup"><span data-stu-id="9ded3-148">**Why doesn’t the forecast change when I make changes to my resources?**</span></span>  
<span data-ttu-id="9ded3-149">预测模型需要几天的时间来考虑帐户的更改，并且不会根据资源的变化做出即时投影</span><span class="sxs-lookup"><span data-stu-id="9ded3-149">The forecast model requires a couple of days to account for changes in the account and does not make immediate projections based on change in resources</span></span>  
<span data-ttu-id="9ded3-150">对于更大的资源增加或减少的步骤，模型会花更长的时间来调整这些更改，以应对异常情况</span><span class="sxs-lookup"><span data-stu-id="9ded3-150">For larger steps of increase or decrease in resources, the model will take slightly longer to adjust to these changes to account for anomalies</span></span>

<span data-ttu-id="9ded3-151">**为什么我的预测会在我进行保留或市场购买后增加？**</span><span class="sxs-lookup"><span data-stu-id="9ded3-151">**Why does my forecast increase after I make a reservation or Marketplace purchase?**</span></span>  
<span data-ttu-id="9ded3-152">预测模型会考虑您的 "实际成本"，而不是单独考虑使用和购买。对于一次性购买，模型将在10天后减少预测，以导致成本突然增加</span><span class="sxs-lookup"><span data-stu-id="9ded3-152">The forecast model considers your 'Actual Cost' and does not account for usage and purchase separately.For a one-time purchase, the model will decrease the projections after 10 days to account for the sudden increase in costs</span></span>

<span data-ttu-id="9ded3-153">**我想查看单个维的预测 (例如。计量器)**</span><span class="sxs-lookup"><span data-stu-id="9ded3-153">**I want to see forecasts for a single dimension (eg. Meter)**</span></span>  
<span data-ttu-id="9ded3-154">预测目前支持总成本预测，而不支持单个仪表。</span><span class="sxs-lookup"><span data-stu-id="9ded3-154">Forecast currently supports total cost projections and not for individual meters.</span></span> <span data-ttu-id="9ded3-155">因此，当 "分组依据" 维度时，预测将是维中所有项目的总计</span><span class="sxs-lookup"><span data-stu-id="9ded3-155">Hence, when 'Grouped by' a dimension, the projections will be for total of all items in the dimension</span></span>

<span data-ttu-id="9ded3-156">**建议的文档**</span><span class="sxs-lookup"><span data-stu-id="9ded3-156">**Recommended Documents**</span></span>

- [<span data-ttu-id="9ded3-157">什么是 Azure 成本管理？</span><span class="sxs-lookup"><span data-stu-id="9ded3-157">What is Azure Cost Management?</span></span>](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="9ded3-158">Azure 成本管理最佳实践</span><span class="sxs-lookup"><span data-stu-id="9ded3-158">Azure Cost Management best practices</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="9ded3-159">分析成本和支出</span><span class="sxs-lookup"><span data-stu-id="9ded3-159">Analyze your costs and spending</span></span>](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="9ded3-160">使用成本分析探索和分析成本</span><span class="sxs-lookup"><span data-stu-id="9ded3-160">Explore and analyze costs with Cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="9ded3-161">Azure 成本管理：定价</span><span class="sxs-lookup"><span data-stu-id="9ded3-161">Azure Cost Management: Pricing</span></span>](https://azure.microsoft.com/services/cost-management/#pricing)
- [<span data-ttu-id="9ded3-162">查看成本分析中的成本</span><span class="sxs-lookup"><span data-stu-id="9ded3-162">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [<span data-ttu-id="9ded3-163">视频教程：在 Azure 门户中创建预算</span><span class="sxs-lookup"><span data-stu-id="9ded3-163">Video tutorial: Create a budget in the Azure portal</span></span>](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [<span data-ttu-id="9ded3-164">查看和自定义预算的先决条件</span><span class="sxs-lookup"><span data-stu-id="9ded3-164">Prerequisites for viewing and customizing budgets</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [<span data-ttu-id="9ded3-165">创建和管理预算</span><span class="sxs-lookup"><span data-stu-id="9ded3-165">Create and manage budgets</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [<span data-ttu-id="9ded3-166">使用 Azure 操作组和预算 API 配置自动化</span><span class="sxs-lookup"><span data-stu-id="9ded3-166">Configure automation with Azure Action Groups and Budgets API</span></span>](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [<span data-ttu-id="9ded3-167">使用成本警报监视使用情况和支出</span><span class="sxs-lookup"><span data-stu-id="9ded3-167">Use cost alerts to monitor usage and spending</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="9ded3-168">成本管理最佳实践</span><span class="sxs-lookup"><span data-stu-id="9ded3-168">Cost Management best practices</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

<span data-ttu-id="9ded3-169">**教程视频**</span><span class="sxs-lookup"><span data-stu-id="9ded3-169">**Tutorial videos**</span></span>

- [<span data-ttu-id="9ded3-170">在 Azure 门户中创建预算</span><span class="sxs-lookup"><span data-stu-id="9ded3-170">Create a budget in the Azure portal</span></span>](https://go.microsoft.com/fwlink/?linkid=2146761)
- [<span data-ttu-id="9ded3-171">使用预算 API 和操作组管理成本</span><span class="sxs-lookup"><span data-stu-id="9ded3-171">Manage costs with the Budgets API and Action Groups</span></span>](https://go.microsoft.com/fwlink/?linkid=2147038)