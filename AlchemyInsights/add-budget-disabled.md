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
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954652"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>为什么我禁用了"添加预算"按钮？

若要创建预算，您需要以下权限之一：

- 管理组、订阅、资源组作用域
- 成本管理参与者
- 所有者
- 参与者
- Enterprise仅客户：注册、部门、帐户作用域
- 注册管理员 (注册范围设置) 
- 部门管理员 (部门范围内设置) 
- 帐户所有者 (作用域设置预算) 
- 仅新式客户协议：计费帐户、计费配置文件、发票部分范围
- Azure 订阅创建者

**当当当月的成本已超预算时，我创建了一个预算。为什么我没有收到警报？**  
如果在创建预算时已超出给定成本阈值，将不会触发警报。 新周期开始后，如果超出阈值，将触发警报。

**当超过定义的一个预算警报阈值后，我应何时收到警报？**  
每 4 小时评估一次预算。 使用数据到达预算系统至少需要 8 小时。 考虑到这一点，超过阈值后，警报可能需要 12 小时才能触发。

**Why is the Start date button disabled when I select a Month or Billing month reset period？**  
预算与当前日历月或当前计费周期 (（如果选择了"计费月份") ）。 因此，我们将预先填充此值。

**为什么我在预算创建体验中看不到我成本的图形？**  
我们至少需要 2 个月的成本数据，然后才能呈现图形来帮助你创建预算。

**为什么我无法针对刚创建的订阅设置预算？**  
创建订阅后，在针对数据设置预算之前，需要 24-48 小时处理数据。

**预算 API 资源**

- [预算 API v1：](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)提供用于创建和更新预算的操作。 使用预算 API，可以设置预算阈值，并配置多个警报以在接近该阈值时触发。 警报可以触发电子邮件或 Azure 操作组以执行自动化。 注意：此 API 筛选与查询 API 筛选/维度不一致。
- [预算 API v2：](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)使用比 v1 更高的成本筛选功能创建预算。 筛选与查询和维度 API 中使用的协定一致。 这是建议用于今后使用的预算 API。
- [Dimensions](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)：提供用于获取各种范围内使用情况支持的维度的操作。 使用 Dimensions API，您可以检索维度列表，这些维度可用作使用查询 API 生成查询的输入。
- [查询](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)：提供基于您提供的查询获取聚合成本和使用率数据的操作。 使用查询 API，可以在所有可用维度上指定所需的筛选、排序和分组 (可从 Dimensions API) 。

**预测成本**

**为什么我在成本分析中看不到成本预测？**  
成本分析中可能缺少预测预测的原因有多种，其中一些原因如下：

1. 如果成本数据少于 10 天，将不会加载预测图表。 该模型需要至少 10 天的最近成本数据，以用于准确的预测
2. 如果选择了历史日期，则预测图表将不可见。 Please select a date range with future dates for the forecast chart to be displayed
3. 如果你的帐户具有多种货币，预测图表将仅针对"所有成本以美元为单位"的项目成本

**为什么我对资源进行更改时预测没有变化？**  
预测模型需要几天的时间来考虑帐户中的更改，并且不会根据资源更改立即进行预测  
对于资源增加或减少的较大步骤，模型需要更长的调整时间以适应这些更改，以考虑异常

**为什么我在预订或市场购买后预测会增加？**  
预测模型会考虑你的"实际成本"，并不单独考虑使用情况和购买。对于一次购买，该模型将在 10 天后减少预测，以说明成本的突然增加

**我想查看单个维度预测，例如 (预测。指示器)**  
预测当前支持总成本预测，而非单米预测。 因此，当"分组者"一个维度时，投影将为维度中所有项的总计

**推荐文档**

- [什么是 Azure 成本管理？](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure 成本管理最佳做法](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [分析成本和费用](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [使用成本分析探索和分析成本](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure 成本管理：定价](https://azure.microsoft.com/services/cost-management/#pricing)
- [查看成本分析中的成本](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [视频教程：在 Azure 门户创建预算](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [查看和自定义预算的先决条件](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [创建和管理预算](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [使用 Azure 操作组和预算 API 配置自动化](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [使用成本警报监视使用情况和费用](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [成本管理最佳做法](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**教程视频**

- [在 Azure 门户创建预算](https://go.microsoft.com/fwlink/?linkid=2146761)
- [使用预算 API 和操作组管理成本](https://go.microsoft.com/fwlink/?linkid=2147038)