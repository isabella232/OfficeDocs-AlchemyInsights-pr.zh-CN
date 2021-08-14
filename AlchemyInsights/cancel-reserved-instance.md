---
title: 取消保留
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 8d0a6a37a244e817472c3949109481a30d80328b7353806905e05c547e196ea0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931223"
---
# <a name="cancelling-reservation"></a>取消保留

- **自助服务：** 可自行使用 [Azure 门户](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)取消或更换保留实例。 选择保留，然后单击退款或交换。 请注意，你必须持有“保留订单”的所有者访问权限才能进行交换或退款。 仅持有对“保留”的访问权限将不允许你进行退款或交换。 请求“保留订单”所有者授予你对“保留订单”的访问权限
- **交换策略：** 你可以与同一类型的另一保留进行交换，交换保留将 **不收到处罚**。 新保留的整体承诺应大于已交换保留的退款金额与未来的每月付款（如果适用）
- **退款政策：** 退款总额和已取消的未来付款情况在长达 12 个月的滚动窗口内不得超过 $50,000 美元。 对于退款，我们 **目前不实施任何处罚收费**，但可能在未来的退款中对其计费  
    **例外：** 自助服务交换和取消功能不适用于美国政府企业协议客户
- **API / PS / CLI** 支持不可用于取消和退款 [针对 Azure 保留的自助服务交换和退款](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- 自助服务交换和取消功能不可用于美国政府企业协议客户。 支持其他美国政府订阅类型（包括“即付即用”和 CSP）

了解详细信息：[如何处理退货和交换事务](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
了解详细信息：[交换和退款政策](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
其他问题：[访问保留的实例文档](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**交换现有保留实例（自助服务）**

可将现有保留与同一类型的另一保留进行交换。 如果不再需要保留，你也可以退款，每年最高 $50,000 美元。 自助服务交换和取消功能不可用于美国政府企业协议客户。 支持其他美国政府订阅类型（包括“即付即用”和 CSP）。 你必须持有“保留订单”的所有者访问权限才能对现有保留进行交换或退款。

以下步骤将提供完成事务的指导过程

1. 登录到 [Azure 门户](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)。 选择要退款的保留，然后单击“**交换**”
2. 选择要购买的 VM 产品并键入数量。 确保新的购买总额超出退货总额 [在购买之前确定正确的大小](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. 检查和完成事务

**保留实例的退款**

若要退款保留，请转到“**保留详细信息**”，然后单击“**退款**”

**按照比例的退款：**

**退款和交换的按照配额和最低要求示例**  
预付保留示例：

- 你在 1 月 1 日花费 $120 购买了为期一年的 R1
- 在 4 月 7 日，你希望退款或交换此保留
- 由于保留已活跃 97 天，你将获得 (1-97/365) * $120 的退款。 （即 $88.1）。 目前没有退款处罚
- 如果要交换，新的购买应高于 $88.1
- 目前退款不会受到处罚

**计费套餐保留示例：**

- 你购买了为期一年的 RI（每月支付 $10）
- 在 4 月 7 日，你希望退款或交换此保留
- 由于上次的付款发生在 7 天前，你将获得 (1-7/31) * $10 的退款。(即 $7.74)
- 所取消的未来付款是 $80。 目前没有退款处罚
- 此取消将从你的 $50,000 退款限度中扣除 $87.74
- 如果进行交换，则新购买的总额应大于 $87.74

**推荐文档**

- [如何处理退货和交换事务](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [交换和退款政策](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)