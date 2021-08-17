---
title: 预留实例购买账单
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
ms.openlocfilehash: 00565470de388165e64c45879c22fd5064b4adc695151edaf58878f38a481ff2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104010"
---
# <a name="billing-for-reserved-instance-purchase"></a>预留实例购买账单

预留实例购买将按照与您在购买时选择的订阅相关的付款方式进行收费。 订阅类型必须是企业协议（优惠号码： MS-CHAP，AZR-0017P）、即用即付支付（优惠号码： MS-CHAP-AZR-0003P）、Microsoft 客户协议或 CSP。

- 对于企业订阅，费用从注册的货币承诺余额中扣除或作为超额收费
- 对于即用即付订阅，收费通过订阅上的信用卡或发票付款方式计费

**取消保留**

- **自助服务：** 可自行使用 [Azure 门户](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)取消或更换保留实例。 选择保留，然后单击退款或交换。 请注意，你必须持有“保留订单”的所有者访问权限才能进行交换或退款。 仅持有对“保留”的访问权限将不允许你进行退款或交换。 请求“保留订单”所有者授予你对“保留订单”的访问权限
- **交换策略：** 你可以与同一类型的另一保留进行交换，交换保留将 **不收到处罚**。 新保留的整体承诺应大于已交换保留的退款金额与未来的每月付款（如果适用）
- **退款政策：** 退款总额和已取消的未来付款情况在长达 12 个月的滚动窗口内不得超过 $50,000 美元。 对于退款，我们 **目前不实施任何处罚收费**，但可能在未来的退款中对其计费

**例外：** 自助服务交换和取消功能不适用于美国政府企业协议客户

- **API / PS / CLI** 支持不可用于取消和退款 [针对 Azure 保留的自助服务交换和退款](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- 自助服务交换和取消功能不可用于美国政府企业协议客户。 支持其他美国政府订阅类型（包括“即付即用”和 CSP）

了解更多 ：[如何处理退回](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)和 exchange 交易 了解更多 ： [Exchange 和退款策略](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)其他问题：[访问预留实例文档](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**交换现有保留实例（自助服务）**

可将现有保留与同一类型的另一保留进行交换。 如果不再需要保留，你也可以退款，每年最高 $50,000 美元。 自助服务交换和取消功能不可用于美国政府企业协议客户。 支持其他美国政府订阅类型（包括“即付即用”和 CSP）。 你必须持有“保留订单”的所有者访问权限才能对现有保留进行交换或退款。

以下步骤将提供完成事务的指导过程

1.登录到 Azure [门户](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)。 选择要退款的预订，然后单击"Exchange  2"。选择要购买的 VM 产品并键入数量。 确保新购买总额大于返回总数 在购买前确定 [正确大小](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)。
3.查看并完成事务

**保留实例的退款**

若要退款保留，请转到“**保留详细信息**”，然后单击“**退款**”

**按照比例的退款：**

**Pro退款和交换的最低要求示例** 预先预订示例：

- 你在 1 月 1 日花费 $120 购买了为期一年的 R1
- 在 4 月 7 日，你希望退款或交换此保留
- 由于保留已活跃 97 天，你将获得 (1-97/365) * $120 的退款。 （即 $88.1）。 目前没有退款处罚
- 如果要交换，新的购买应高于 $88.1
- 目前退款不会受到处罚

**计费套餐保留示例：**

- 你购买了为期一年的 RI（每月支付 $10）
- 在 4 月 7 日，你希望退款或交换此保留
- 由于上次的付款发生在 7 天前，你将获得 (1-7/31) * $10 的退款。 （即 $7.74）
- 所取消的未来付款是 $80。 目前没有退款处罚
- 此取消将从你的 $50,000 退款限度中扣除 $87.74
- 如果进行交换，则新购买的总额应大于 $87.74

**无法查看上一个计费周期的发票**

可能看不到发票的一些可能原因：

- 订阅的每月信用额度未超过，或者有免费试用版。 仅当你付款时，才生成发票
- 订阅 Azure 的时间少于 30 天
- 尚未生成发票。 等待计费周期结束
- 如果你不是帐户管理员，则旧的发票可能不可用

**从 Azure 门户门户下载 (.pdf)**

- 作为有权访问发票的用户，[](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)从 Azure 门户的订阅页面[选择订阅](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- 选择 **发票**
- 单击“**下载发票**”以查看 PDF 发票的副本。 如果显示“**不可用**”，请参阅“[为何无法查看上次帐单周期的发票？](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)”

**在电子邮件服务中接收 (.pdf)**

- 从订阅页面 [选择](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) 你的订阅。 单击 **"发票"，** 然后"通过电子邮件发送我的发票"
- 单击 **"选择加入** "并接受条款。 你必须选择加入你拥有的每个订阅

注意：如果按照步骤操作后没有收到电子邮件，请确保你的电子邮件地址在个人资料的通信首选项 [中是正确的](https://account.windowsazure.com/profile)

**从 Azure 门户下载使用情况数据**

- 以帐户 [管理员角色登录到 Azure](https://account.windowsazure.com/Subscriptions) [帐户中心](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)
- 选择要获取发票和使用情况信息的订阅
- 选择 **帐单历史记录**
- 选择 **"查看当前** 语句"以查看生成估计时的费用估计
- 选择 **"下载** 使用情况"以将每日使用率数据下载为 CSV 文件。 如果看到两个版本可用，请下载版本 2

其他问题：[访问保留的实例文档](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**推荐文档**

- [计费基础知识](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [了解如何应用预留实例折扣](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [下载或查看 Azure 帐单发票和每日使用情况数据](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [了解如何应用预留实例折扣](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [了解"按时付费"订阅的预留实例使用情况](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [了解注册的预留实例Enterprise使用情况](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Windows预留实例中不包括的软件成本](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [合作伙伴中心云解决方案提供商计划云解决方案提供商 (预留) 实例](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)