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
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>为什么 "添加预算" 按钮对我是禁用的？

若要创建预算，您需要以下权限之一：

- 管理组、订阅、资源组作用域
- 成本管理参与者
- 所有者
- 参与者
- 仅企业客户：注册、部门、帐户范围
- 注册管理员 (在注册作用域设置预算) 
- 部门管理员 (设置部门范围内的预算) 
- 帐户所有者 (设置 "帐户" 范围内的预算) 
- 仅限新式客户协议：帐单帐户、帐单配置文件、发票部分范围
- Azure 订阅创建程序

**当我的当前月成本已过预算时，我创建了预算。为什么我没有收到通知？**  
如果您在创建预算时已超出给定的成本阈值，则不会触发预警。 新周期开始后，如果您违反阈值，则会触发警报。

**我在超过我定义的某个预算警报阈值后何时应该收到通知？**  
每4小时对预算进行一次评估。 使用率数据最少需要8小时才能到达预算系统。 在此情况下，在超过阈值后触发警报可能需要等待12个小时。

**为什么在我选择一个月或帐单重置时段时禁用开始日期按钮？**  
预算与当前的日历月或当前帐单期对齐 (在) 中选择计费月的情况下。 因此，我们为你预填充此值。

**为什么我在预算创建体验中看不到我的成本关系图？**  
我们至少需要2个月的成本数据，才能呈现可帮助您创建预算的图形。

**为什么我无法针对刚刚创建的订阅设置预算？**  
创建订阅后，在为数据设置预算之前，数据需要24-48 小时才能处理。

**预算 API 资源**

- [预算 API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)：提供用于创建和更新预算的操作。 使用预算 API，您可以设置预算阈值，并配置多个警报以在您接近该阈值时触发。 警报可触发电子邮件或 Azure 操作组以执行自动化。 注意：此 API 的筛选不与查询 API 筛选/维度相一致。
- [预算 API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)：使用高于 v1 的成本筛选功能创建预算。 筛选与我们的查询和维度 Api 中使用的约定相适应。 这是建议的预算 API，以供将来使用。
- [维度](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)：提供在各种范围内为您的使用获取受支持的维度的操作。 使用维度 API，您可以检索可用作在查询 API 中生成查询的输入的维度列表。
- [查询](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)：提供根据您提供的查询来获取聚合成本和使用情况数据的操作。 使用查询 API，您可以指定所需的筛选，在所有可用维度上进行排序和分组， (可从维度 API) 访问。

**预测成本**

**为什么我在成本分析中看不到我对成本的预测？**  
在成本分析中可能缺少预测计划的多个原因，其中一些原因如下：

1. 如果您的成本数据少于10天，则不会加载预测图表。 模型需要至少10天的最近成本数据才能实现准确的预测
2. 如果您已选择历史日期，则预测图表将不可见。 请选择要显示的预测图表的日期范围和未来日期
3. 如果你的帐户有多种货币，则预测图表将仅对 "所有费用都是 USD" 的成本进行项目

**为什么在我对我的资源进行更改时预测不会发生变化？**  
预测模型需要几天的时间来考虑帐户的更改，并且不会根据资源的变化做出即时投影  
对于更大的资源增加或减少的步骤，模型会花更长的时间来调整这些更改，以应对异常情况

**为什么我的预测会在我进行保留或市场购买后增加？**  
预测模型会考虑您的 "实际成本"，而不是单独考虑使用和购买。对于一次性购买，模型将在10天后减少预测，以导致成本突然增加

**我想查看单个维的预测 (例如。计量器)**  
预测目前支持总成本预测，而不支持单个仪表。 因此，当 "分组依据" 维度时，预测将是维中所有项目的总计

**建议的文档**

- [什么是 Azure 成本管理？](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure 成本管理最佳实践](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [分析成本和支出](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [使用成本分析探索和分析成本](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure 成本管理：定价](https://azure.microsoft.com/services/cost-management/#pricing)
- [查看成本分析中的成本](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [视频教程：在 Azure 门户中创建预算](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [查看和自定义预算的先决条件](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [创建和管理预算](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [使用 Azure 操作组和预算 API 配置自动化](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [使用成本警报监视使用情况和支出](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [成本管理最佳实践](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**教程视频**

- [在 Azure 门户中创建预算](https://go.microsoft.com/fwlink/?linkid=2146761)
- [使用预算 API 和操作组管理成本](https://go.microsoft.com/fwlink/?linkid=2147038)