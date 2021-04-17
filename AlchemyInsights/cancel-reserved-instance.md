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
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819682"
---
# <a name="cancelling-reservation"></a><span data-ttu-id="b77a7-102">取消保留</span><span class="sxs-lookup"><span data-stu-id="b77a7-102">Cancelling Reservation</span></span>

- <span data-ttu-id="b77a7-103">**自助服务：** 可自行使用 [Azure 门户](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)取消或更换保留实例。</span><span class="sxs-lookup"><span data-stu-id="b77a7-103">**Self-service:** You can cancel or exchange a reserved instance yourself using [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade).</span></span> <span data-ttu-id="b77a7-104">选择保留，然后单击退款或交换。</span><span class="sxs-lookup"><span data-stu-id="b77a7-104">Select the reservation and click on refund or exchange.</span></span> <span data-ttu-id="b77a7-105">请注意，你必须持有“保留订单”的所有者访问权限才能进行交换或退款。</span><span class="sxs-lookup"><span data-stu-id="b77a7-105">Note that you must have owner access on the Reservation Order to exchange or refund.</span></span> <span data-ttu-id="b77a7-106">仅持有对“保留”的访问权限将不允许你进行退款或交换。</span><span class="sxs-lookup"><span data-stu-id="b77a7-106">Access to only the Reservation will not let you proceed with refund or exchange.</span></span> <span data-ttu-id="b77a7-107">请求“保留订单”所有者授予你对“保留订单”的访问权限</span><span class="sxs-lookup"><span data-stu-id="b77a7-107">Ask the Reservation Order owner to give you owner access to the Reservation Order</span></span>
- <span data-ttu-id="b77a7-108">**交换策略：** 你可以与同一类型的另一保留进行交换，交换保留将 **不收到处罚**。</span><span class="sxs-lookup"><span data-stu-id="b77a7-108">**Exchange policy:** You can exchange a reservation for another reservation of the same type – there are **no penalties** on reservation exchange.</span></span> <span data-ttu-id="b77a7-109">新保留的整体承诺应大于已交换保留的退款金额与未来的每月付款（如果适用）</span><span class="sxs-lookup"><span data-stu-id="b77a7-109">The total commitment with new reservation should be greater than the sum of exchanged reservation’s refund amount and the future monthly payments (if applicable)</span></span>
- <span data-ttu-id="b77a7-110">**退款政策：** 退款总额和已取消的未来付款情况在长达 12 个月的滚动窗口内不得超过 $50,000 美元。</span><span class="sxs-lookup"><span data-stu-id="b77a7-110">**Refund policy:** Sum of refund and the cancelled future payments cannot exceed $50,000 USD in a 12-month rolling window.</span></span> <span data-ttu-id="b77a7-111">对于退款，我们 **目前不实施任何处罚收费**，但可能在未来的退款中对其计费</span><span class="sxs-lookup"><span data-stu-id="b77a7-111">We are **currently not charging any penalty** on refunds but could charge it on future refunds</span></span>  
    <span data-ttu-id="b77a7-112">**例外：** 自助服务交换和取消功能不适用于美国政府企业协议客户</span><span class="sxs-lookup"><span data-stu-id="b77a7-112">**Exceptions:** Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers</span></span>
- <span data-ttu-id="b77a7-113">**API / PS / CLI** 支持不可用于取消和退款 [针对 Azure 保留的自助服务交换和退款](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="b77a7-113">**API / PS / CLI** support is not available for cancellation and refunds [Self-service exchanges and refunds for Azure Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- <span data-ttu-id="b77a7-114">自助服务交换和取消功能不可用于美国政府企业协议客户。</span><span class="sxs-lookup"><span data-stu-id="b77a7-114">Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers.</span></span> <span data-ttu-id="b77a7-115">支持其他美国政府订阅类型（包括“即付即用”和 CSP）</span><span class="sxs-lookup"><span data-stu-id="b77a7-115">Other US Government subscription types including Pay-As-You-Go and CSP are supported</span></span>

<span data-ttu-id="b77a7-116">了解详细信息：[如何处理退货和交换事务](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)</span><span class="sxs-lookup"><span data-stu-id="b77a7-116">Learn more : [How return and exchange transactions are processed](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)</span></span>  
<span data-ttu-id="b77a7-117">了解详细信息：[交换和退款政策](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)</span><span class="sxs-lookup"><span data-stu-id="b77a7-117">Learn more : [Exchange and Refund policies](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)</span></span>  
<span data-ttu-id="b77a7-118">其他问题：[访问保留的实例文档](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="b77a7-118">Other questions: [Visit reserved instance docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="b77a7-119">**交换现有保留实例（自助服务）**</span><span class="sxs-lookup"><span data-stu-id="b77a7-119">**Exchange an existing reserved instance (Self-service)**</span></span>

<span data-ttu-id="b77a7-120">可将现有保留与同一类型的另一保留进行交换。</span><span class="sxs-lookup"><span data-stu-id="b77a7-120">You can exchange a reservation for another reservation of the same type.</span></span> <span data-ttu-id="b77a7-121">如果不再需要保留，你也可以退款，每年最高 $50,000 美元。</span><span class="sxs-lookup"><span data-stu-id="b77a7-121">You can also refund a reservation, up to $50,000 USD per year, if you no longer need it.</span></span> <span data-ttu-id="b77a7-122">自助服务交换和取消功能不可用于美国政府企业协议客户。</span><span class="sxs-lookup"><span data-stu-id="b77a7-122">Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers.</span></span> <span data-ttu-id="b77a7-123">支持其他美国政府订阅类型（包括“即付即用”和 CSP）。</span><span class="sxs-lookup"><span data-stu-id="b77a7-123">Other US Government subscription types including Pay-As-You-Go and CSP are supported.</span></span> <span data-ttu-id="b77a7-124">你必须持有“保留订单”的所有者访问权限才能对现有保留进行交换或退款。</span><span class="sxs-lookup"><span data-stu-id="b77a7-124">You must have owner access on the Reservation Order to exchange or refund an existing reservation.</span></span>

<span data-ttu-id="b77a7-125">以下步骤将提供完成事务的指导过程</span><span class="sxs-lookup"><span data-stu-id="b77a7-125">The following steps will guide on the procedure to complete the transaction</span></span>

1. <span data-ttu-id="b77a7-126">登录到 [Azure 门户](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)。</span><span class="sxs-lookup"><span data-stu-id="b77a7-126">Log in to your [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade).</span></span> <span data-ttu-id="b77a7-127">选择要退款的保留，然后单击“**交换**”</span><span class="sxs-lookup"><span data-stu-id="b77a7-127">Select the reservations that you want to refund and click **Exchange**</span></span>
2. <span data-ttu-id="b77a7-128">选择要购买的 VM 产品并键入数量。</span><span class="sxs-lookup"><span data-stu-id="b77a7-128">Select the VM product that you want to purchase and type a quantity.</span></span> <span data-ttu-id="b77a7-129">确保新的购买总额超出退货总额 [在购买之前确定正确的大小](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)</span><span class="sxs-lookup"><span data-stu-id="b77a7-129">Make sure that the new purchase total is more than the return total [Determine the right size before you purchase](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)</span></span>
3. <span data-ttu-id="b77a7-130">检查和完成事务</span><span class="sxs-lookup"><span data-stu-id="b77a7-130">Review and complete the transaction</span></span>

<span data-ttu-id="b77a7-131">**保留实例的退款**</span><span class="sxs-lookup"><span data-stu-id="b77a7-131">**Refund for a reserved instance**</span></span>

<span data-ttu-id="b77a7-132">若要退款保留，请转到“**保留详细信息**”，然后单击“**退款**”</span><span class="sxs-lookup"><span data-stu-id="b77a7-132">To refund a reservation, go to **Reservation Details** and click **Refund**</span></span>

<span data-ttu-id="b77a7-133">**按照比例的退款：**</span><span class="sxs-lookup"><span data-stu-id="b77a7-133">**Pro-rated refund:**</span></span>

<span data-ttu-id="b77a7-134">**退款和交换的按照配额和最低要求示例**</span><span class="sxs-lookup"><span data-stu-id="b77a7-134">**Pro-ration and minimum requirement examples for refund and exchange**</span></span>  
<span data-ttu-id="b77a7-135">预付保留示例：</span><span class="sxs-lookup"><span data-stu-id="b77a7-135">Upfront reservation example:</span></span>

- <span data-ttu-id="b77a7-136">你在 1 月 1 日花费 $120 购买了为期一年的 R1</span><span class="sxs-lookup"><span data-stu-id="b77a7-136">You purchase a one-year term RI for $120 on January 1</span></span>
- <span data-ttu-id="b77a7-137">在 4 月 7 日，你希望退款或交换此保留</span><span class="sxs-lookup"><span data-stu-id="b77a7-137">On April 7th you want to refund or exchange this reservation</span></span>
- <span data-ttu-id="b77a7-138">由于保留已活跃 97 天，你将获得 (1-97/365) \* $120 的退款。</span><span class="sxs-lookup"><span data-stu-id="b77a7-138">Since the reservation has been live for 97 days, you will get (1-97/365) \* $120 back.</span></span> <span data-ttu-id="b77a7-139">（即 $88.1）。</span><span class="sxs-lookup"><span data-stu-id="b77a7-139">(i.e. $88.1).</span></span> <span data-ttu-id="b77a7-140">目前没有退款处罚</span><span class="sxs-lookup"><span data-stu-id="b77a7-140">There is currently no penalty on refunds</span></span>
- <span data-ttu-id="b77a7-141">如果要交换，新的购买应高于 $88.1</span><span class="sxs-lookup"><span data-stu-id="b77a7-141">If exchanging, your new purchase should be greater than $88.1</span></span>
- <span data-ttu-id="b77a7-142">目前退款不会受到处罚</span><span class="sxs-lookup"><span data-stu-id="b77a7-142">There is no penalty on refunds currently</span></span>

<span data-ttu-id="b77a7-143">**计费套餐保留示例：**</span><span class="sxs-lookup"><span data-stu-id="b77a7-143">**Billing plan reservation example:**</span></span>

- <span data-ttu-id="b77a7-144">你购买了为期一年的 RI（每月支付 $10）</span><span class="sxs-lookup"><span data-stu-id="b77a7-144">You purchase a one-year term RI for $10 per month</span></span>
- <span data-ttu-id="b77a7-145">在 4 月 7 日，你希望退款或交换此保留</span><span class="sxs-lookup"><span data-stu-id="b77a7-145">On April 7th you want to refund or exchange this reservation</span></span>
- <span data-ttu-id="b77a7-146">由于上次的付款发生在 7 天前，你将获得 (1-7/31) \* $10 的退款。</span><span class="sxs-lookup"><span data-stu-id="b77a7-146">Since the last payment happened 7 days, you will get (1-7/31) \* $10 back.</span></span> <span data-ttu-id="b77a7-147">（即 $7.74）</span><span class="sxs-lookup"><span data-stu-id="b77a7-147">(i.e. $7.74)</span></span>
- <span data-ttu-id="b77a7-148">所取消的未来付款是 $80。</span><span class="sxs-lookup"><span data-stu-id="b77a7-148">The future payments cancelled are $ 80.</span></span> <span data-ttu-id="b77a7-149">目前没有退款处罚</span><span class="sxs-lookup"><span data-stu-id="b77a7-149">There is currently no penalty on refunds</span></span>
- <span data-ttu-id="b77a7-150">此取消将从你的 $50,000 退款限度中扣除 $87.74</span><span class="sxs-lookup"><span data-stu-id="b77a7-150">This cancellation will deduct $87.74 from you’re the $50,000 refund limit</span></span>
- <span data-ttu-id="b77a7-151">如果进行交换，则新购买的总额应大于 $87.74</span><span class="sxs-lookup"><span data-stu-id="b77a7-151">If exchanging, the total value of new purchase should be greater than $87.74</span></span>

<span data-ttu-id="b77a7-152">**推荐文档**</span><span class="sxs-lookup"><span data-stu-id="b77a7-152">**Recommended Documents**</span></span>

- [<span data-ttu-id="b77a7-153">如何处理退货和交换事务</span><span class="sxs-lookup"><span data-stu-id="b77a7-153">How return and exchange transactions are processed</span></span>](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [<span data-ttu-id="b77a7-154">交换和退款政策</span><span class="sxs-lookup"><span data-stu-id="b77a7-154">Exchange and Refund policies</span></span>](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)