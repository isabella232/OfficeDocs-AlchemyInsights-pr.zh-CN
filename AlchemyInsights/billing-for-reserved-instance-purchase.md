---
title: 预留实例购买的计费
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
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820312"
---
# <a name="billing-for-reserved-instance-purchase"></a>预留实例购买的计费

预留实例购买收取与购买时选择的订阅绑定的付款方式的费用。 订阅类型必须是企业协议 (产品/服务编号：MS-AZR-0017P) 、即付即用 (产品/服务编号：MS-AZR-0003P) 、Microsoft 客户协议或云解决方案提供商。

- 对于企业订阅，费用从注册的货币承诺余额中减去，或收取过度费用
- 对于"按天付费"订阅，费用通过订阅的信用卡或发票付款方式计费

**取消预订**

- **自助服务：** 可以使用 Azure 门户自己取消或交换 [预留实例](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)。 选择预订并单击退款或兑换。 请注意，你必须对预订订单拥有所有者访问权限才能兑换或退款。 仅访问预订将不允许你继续退款或兑换。 让预订订单所有者授予你所有者对预订订单的访问权限
- **Exchange 策略：** 你可以将预订交换为同一类型的另一个预订 ， **对预订** 交换没有任何处罚。 新预订的承诺总额应大于已兑换预订的退款金额以及以后每月付款 (如果适用) 
- **退款策略：** 在 12 个月的滚动窗口中，退款和取消的未来付款不能超过 50，000 美元。 我们 **目前不对退款** 收取任何罚款，但可能会收取以后的退款

**例外情况：** 自助服务交换和取消功能不适用于美国政府企业协议客户

- **API / PS / CLI** 支持不适用于取消和退款自助服务交换和 Azure [预订退款](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- 自助服务交换和取消功能不适用于美国政府企业协议客户。 支持其他美国政府订阅类型，包括"一付一用"和云解决方案提供商

了解更多 ： [如何处理退回和兑换](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) 交易 了解更多 ： [Exchange and Refund policies](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) 其他问题： [访问预留实例文档](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**Exchange 现有的保留实例 (自助服务)**

可以将预订交换为同一类型的另一个预订。 如果不再需要预订，还可以退款，最高为每年 50，000 美元。 自助服务交换和取消功能不适用于美国政府企业协议客户。 支持其他美国政府订阅类型，包括即付即用和云解决方案提供商。 你必须对预订订单拥有所有者访问权限才能交换现有预订或退款。

以下步骤将指导完成事务的过程

1.登录到 Azure [门户](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)。 选择要退款的预订，然后单击 **"Exchange** 2"。选择要购买的 VM 产品并键入数量。 确保新购买总额大于返回总数 在购买前确定 [正确大小](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)。
3.查看并完成事务

**预留实例的退款**

若要退款预订，请转到预订 **详细信息并****单击退款**

**按比例退款：**

**退款和交换的按比例支付和最低要求示例** 预先预订示例：

- 1 月 1 日购买一年期限 RI，价格为 120 美元
- 在 4 月 7 日，你想要退款或兑换此预订
- 由于预订已预订 97 天， (1-97/365) * $120。  (88.1 美元) 。 目前，退款没有处罚
- 如果交换，你的新购买应大于 $88.1
- 当前退款没有处罚

**计费计划预订示例：**

- 购买一年期限 RI，每月 10 美元
- 在 4 月 7 日，你想要退款或兑换此预订
- 由于上次付款发生 7 天，你 (1-7/31) * $10。  (7.74 美元) 
- 取消的未来付款为 $80。 目前，退款没有处罚
- 此取消将减去 50，000 美元退款限制中的 87.74 美元
- 如果交换，则新购买的总成本应大于 $87.74

**无法查看上一个计费周期的发票**

可能看不到发票的一些可能原因：

- 订阅的每月信用额度未超过，或者有免费试用版。 仅当你付款时，才生成发票
- 订阅 Azure 的时间少于 30 天
- 尚未生成发票。 等待计费周期结束
- 如果你不是帐户管理员，则旧的发票可能不可用

**从 Azure 门户 (.pdf)**

- 作为有权访问发票的用户，[](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)从 Azure 门户的订阅页面[选择订阅](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- 选择 **发票**
- 单击“**下载发票**”以查看 PDF 发票的副本。 如果它表示 **不可用，** 请参阅为什么我看不到上一个计费周期 [的发票？](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**在电子邮件中接收发票 (.pdf)**

- 从订阅页面 [选择](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) 你的订阅。 单击 **"发票"，** 然后"通过电子邮件发送我的发票"
- 单击 **"选择加入** "并接受条款。 你必须选择加入你拥有的每个订阅

注意：如果按照步骤操作后没有收到电子邮件，请确保你的电子邮件地址在个人资料的通信首选项 [中是正确的](https://account.windowsazure.com/profile)

**从 Azure 门户下载使用情况数据**

- 以帐户 [管理员角色登录到 Azure](https://account.windowsazure.com/Subscriptions) [帐户中心](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- 选择要获取发票和使用情况信息的订阅
- 选择 **帐单历史记录**
- 选择 **"查看当前** 语句"以查看生成估计时的费用估计
- 选择 **"下载** 使用情况"以将每日使用率数据下载为 CSV 文件。 如果看到两个版本可用，请下载版本 2

其他问题： [访问预留实例文档](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**推荐文档**

- [计费基础知识](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [了解如何应用预留实例折扣](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [下载或查看 Azure 帐单发票和每日使用情况数据](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [了解如何应用预留实例折扣](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [了解"按时付费"订阅的预留实例使用情况](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [了解企业注册的预留实例使用情况](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [预留实例中不包括 Windows 软件成本](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [合作伙伴中心云解决方案提供商云解决方案提供商计划 (云解决方案) 预留实例](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)