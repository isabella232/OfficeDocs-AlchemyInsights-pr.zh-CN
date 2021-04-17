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
# <a name="billing-for-reserved-instance-purchase"></a><span data-ttu-id="c699c-102">预留实例购买的计费</span><span class="sxs-lookup"><span data-stu-id="c699c-102">Billing for Reserved Instance purchase</span></span>

<span data-ttu-id="c699c-103">预留实例购买收取与购买时选择的订阅绑定的付款方式的费用。</span><span class="sxs-lookup"><span data-stu-id="c699c-103">The reserved instance purchase is charged to the payment method tied to the subscription that you select at the time of purchase.</span></span> <span data-ttu-id="c699c-104">订阅类型必须是企业协议 (产品/服务编号：MS-AZR-0017P) 、即付即用 (产品/服务编号：MS-AZR-0003P) 、Microsoft 客户协议或云解决方案提供商。</span><span class="sxs-lookup"><span data-stu-id="c699c-104">The subscription type must be an enterprise agreement (offer number: MS-AZR-0017P), Pay-As-You-Go (offer number: MS-AZR-0003P), Microsoft Customer Agreement or CSP.</span></span>

- <span data-ttu-id="c699c-105">对于企业订阅，费用从注册的货币承诺余额中减去，或收取过度费用</span><span class="sxs-lookup"><span data-stu-id="c699c-105">For an enterprise subscription, the charges are deducted from the enrollment's monetary commitment balance or charged as overage</span></span>
- <span data-ttu-id="c699c-106">对于"按天付费"订阅，费用通过订阅的信用卡或发票付款方式计费</span><span class="sxs-lookup"><span data-stu-id="c699c-106">For Pay-As-You-Go subscription, the charges are billed to the credit card or invoice payment method on the subscription</span></span>

<span data-ttu-id="c699c-107">**取消预订**</span><span class="sxs-lookup"><span data-stu-id="c699c-107">**Cancelling Reservation**</span></span>

- <span data-ttu-id="c699c-108">**自助服务：** 可以使用 Azure 门户自己取消或交换 [预留实例](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)。</span><span class="sxs-lookup"><span data-stu-id="c699c-108">**Self-service:** You can cancel or exchange a reserved instance yourself using [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade).</span></span> <span data-ttu-id="c699c-109">选择预订并单击退款或兑换。</span><span class="sxs-lookup"><span data-stu-id="c699c-109">Select the reservation and click on refund or exchange.</span></span> <span data-ttu-id="c699c-110">请注意，你必须对预订订单拥有所有者访问权限才能兑换或退款。</span><span class="sxs-lookup"><span data-stu-id="c699c-110">Note that you must have owner access on the Reservation Order to exchange or refund.</span></span> <span data-ttu-id="c699c-111">仅访问预订将不允许你继续退款或兑换。</span><span class="sxs-lookup"><span data-stu-id="c699c-111">Access to only the Reservation will not let you proceed with refund or exchange.</span></span> <span data-ttu-id="c699c-112">让预订订单所有者授予你所有者对预订订单的访问权限</span><span class="sxs-lookup"><span data-stu-id="c699c-112">Ask the Reservation Order owner to give you owner access to the Reservation Order</span></span>
- <span data-ttu-id="c699c-113">**Exchange 策略：** 你可以将预订交换为同一类型的另一个预订 ， **对预订** 交换没有任何处罚。</span><span class="sxs-lookup"><span data-stu-id="c699c-113">**Exchange policy:** You can exchange a reservation for another reservation of the same type – there are **no penalties** on reservation exchange.</span></span> <span data-ttu-id="c699c-114">新预订的承诺总额应大于已兑换预订的退款金额以及以后每月付款 (如果适用) </span><span class="sxs-lookup"><span data-stu-id="c699c-114">The total commitment with new reservation should be greater than the sum of exchanged reservation’s refund amount and the future monthly payments (if applicable)</span></span>
- <span data-ttu-id="c699c-115">**退款策略：** 在 12 个月的滚动窗口中，退款和取消的未来付款不能超过 50，000 美元。</span><span class="sxs-lookup"><span data-stu-id="c699c-115">**Refund policy:** Sum of refund and the cancelled future payments cannot exceed $50,000 USD in a 12-month rolling window.</span></span> <span data-ttu-id="c699c-116">我们 **目前不对退款** 收取任何罚款，但可能会收取以后的退款</span><span class="sxs-lookup"><span data-stu-id="c699c-116">We are **currently not charging any penalty** on refunds but could charge it on future refunds</span></span>

<span data-ttu-id="c699c-117">**例外情况：** 自助服务交换和取消功能不适用于美国政府企业协议客户</span><span class="sxs-lookup"><span data-stu-id="c699c-117">**Exceptions:** Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers</span></span>

- <span data-ttu-id="c699c-118">**API / PS / CLI** 支持不适用于取消和退款自助服务交换和 Azure [预订退款](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="c699c-118">**API / PS / CLI** support is not available for cancellation and refunds [Self-service exchanges and refunds for Azure Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- <span data-ttu-id="c699c-119">自助服务交换和取消功能不适用于美国政府企业协议客户。</span><span class="sxs-lookup"><span data-stu-id="c699c-119">Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers.</span></span> <span data-ttu-id="c699c-120">支持其他美国政府订阅类型，包括"一付一用"和云解决方案提供商</span><span class="sxs-lookup"><span data-stu-id="c699c-120">Other US Government subscription types including Pay-As-You-Go and CSP are supported</span></span>

<span data-ttu-id="c699c-121">了解更多 ： [如何处理退回和兑换](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) 交易 了解更多 ： [Exchange and Refund policies](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) 其他问题： [访问预留实例文档](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="c699c-121">Learn more : [How return and exchange transactions are processed](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Learn more : [Exchange and Refund policies](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Other questions: [Visit reserved instance docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="c699c-122">**Exchange 现有的保留实例 (自助服务)**</span><span class="sxs-lookup"><span data-stu-id="c699c-122">**Exchange an existing reserved instance (Self-service)**</span></span>

<span data-ttu-id="c699c-123">可以将预订交换为同一类型的另一个预订。</span><span class="sxs-lookup"><span data-stu-id="c699c-123">You can exchange a reservation for another reservation of the same type.</span></span> <span data-ttu-id="c699c-124">如果不再需要预订，还可以退款，最高为每年 50，000 美元。</span><span class="sxs-lookup"><span data-stu-id="c699c-124">You can also refund a reservation, up to $50,000 USD per year, if you no longer need it.</span></span> <span data-ttu-id="c699c-125">自助服务交换和取消功能不适用于美国政府企业协议客户。</span><span class="sxs-lookup"><span data-stu-id="c699c-125">Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers.</span></span> <span data-ttu-id="c699c-126">支持其他美国政府订阅类型，包括即付即用和云解决方案提供商。</span><span class="sxs-lookup"><span data-stu-id="c699c-126">Other US Government subscription types including Pay-As-You-Go and CSP are supported.</span></span> <span data-ttu-id="c699c-127">你必须对预订订单拥有所有者访问权限才能交换现有预订或退款。</span><span class="sxs-lookup"><span data-stu-id="c699c-127">You must have owner access on the Reservation Order to exchange or refund an existing reservation.</span></span>

<span data-ttu-id="c699c-128">以下步骤将指导完成事务的过程</span><span class="sxs-lookup"><span data-stu-id="c699c-128">The following steps will guide on the procedure to complete the transaction</span></span>

<span data-ttu-id="c699c-129">1.登录到 Azure [门户](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)。</span><span class="sxs-lookup"><span data-stu-id="c699c-129">1.Log in to your [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade).</span></span> <span data-ttu-id="c699c-130">选择要退款的预订，然后单击 **"Exchange** 2"。选择要购买的 VM 产品并键入数量。</span><span class="sxs-lookup"><span data-stu-id="c699c-130">Select the reservations that you want to refund and click **Exchange** 2.Select the VM product that you want to purchase and type a quantity.</span></span> <span data-ttu-id="c699c-131">确保新购买总额大于返回总数 在购买前确定 [正确大小](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)。</span><span class="sxs-lookup"><span data-stu-id="c699c-131">Make sure that the new purchase total is more than the return total [Determine the right size before you purchase](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).</span></span>
<span data-ttu-id="c699c-132">3.查看并完成事务</span><span class="sxs-lookup"><span data-stu-id="c699c-132">3.Review and complete the transaction</span></span>

<span data-ttu-id="c699c-133">**预留实例的退款**</span><span class="sxs-lookup"><span data-stu-id="c699c-133">**Refund for a reserved instance**</span></span>

<span data-ttu-id="c699c-134">若要退款预订，请转到预订 **详细信息并\*\*\*\*单击退款**</span><span class="sxs-lookup"><span data-stu-id="c699c-134">To refund a reservation, go to **Reservation Details** and click **Refund**</span></span>

<span data-ttu-id="c699c-135">**按比例退款：**</span><span class="sxs-lookup"><span data-stu-id="c699c-135">**Pro-rated refund:**</span></span>

<span data-ttu-id="c699c-136">**退款和交换的按比例支付和最低要求示例** 预先预订示例：</span><span class="sxs-lookup"><span data-stu-id="c699c-136">**Pro-ration and minimum requirement examples for refund and exchange** Upfront reservation example:</span></span>

- <span data-ttu-id="c699c-137">1 月 1 日购买一年期限 RI，价格为 120 美元</span><span class="sxs-lookup"><span data-stu-id="c699c-137">You purchase a one-year term RI for $120 on January 1</span></span>
- <span data-ttu-id="c699c-138">在 4 月 7 日，你想要退款或兑换此预订</span><span class="sxs-lookup"><span data-stu-id="c699c-138">On April 7th you want to refund or exchange this reservation</span></span>
- <span data-ttu-id="c699c-139">由于预订已预订 97 天， (1-97/365) \* $120。</span><span class="sxs-lookup"><span data-stu-id="c699c-139">Since the reservation has been live for 97 days, you will get (1-97/365) \* $120 back.</span></span> <span data-ttu-id="c699c-140"> (88.1 美元) 。</span><span class="sxs-lookup"><span data-stu-id="c699c-140">(i.e. $88.1).</span></span> <span data-ttu-id="c699c-141">目前，退款没有处罚</span><span class="sxs-lookup"><span data-stu-id="c699c-141">There is currently no penalty on refunds</span></span>
- <span data-ttu-id="c699c-142">如果交换，你的新购买应大于 $88.1</span><span class="sxs-lookup"><span data-stu-id="c699c-142">If exchanging, your new purchase should be greater than $88.1</span></span>
- <span data-ttu-id="c699c-143">当前退款没有处罚</span><span class="sxs-lookup"><span data-stu-id="c699c-143">There is no penalty on refunds currently</span></span>

<span data-ttu-id="c699c-144">**计费计划预订示例：**</span><span class="sxs-lookup"><span data-stu-id="c699c-144">**Billing plan reservation example:**</span></span>

- <span data-ttu-id="c699c-145">购买一年期限 RI，每月 10 美元</span><span class="sxs-lookup"><span data-stu-id="c699c-145">You purchase a one-year term RI for $10 per month</span></span>
- <span data-ttu-id="c699c-146">在 4 月 7 日，你想要退款或兑换此预订</span><span class="sxs-lookup"><span data-stu-id="c699c-146">On April 7th you want to refund or exchange this reservation</span></span>
- <span data-ttu-id="c699c-147">由于上次付款发生 7 天，你 (1-7/31) \* $10。</span><span class="sxs-lookup"><span data-stu-id="c699c-147">Since the last payment happened 7 days, you will get (1-7/31) \* $10 back.</span></span> <span data-ttu-id="c699c-148"> (7.74 美元) </span><span class="sxs-lookup"><span data-stu-id="c699c-148">(i.e. $7.74)</span></span>
- <span data-ttu-id="c699c-149">取消的未来付款为 $80。</span><span class="sxs-lookup"><span data-stu-id="c699c-149">The future payments cancelled are $ 80.</span></span> <span data-ttu-id="c699c-150">目前，退款没有处罚</span><span class="sxs-lookup"><span data-stu-id="c699c-150">There is currently no penalty on refunds</span></span>
- <span data-ttu-id="c699c-151">此取消将减去 50，000 美元退款限制中的 87.74 美元</span><span class="sxs-lookup"><span data-stu-id="c699c-151">This cancellation will deduct $87.74 from you’re the $50,000 refund limit</span></span>
- <span data-ttu-id="c699c-152">如果交换，则新购买的总成本应大于 $87.74</span><span class="sxs-lookup"><span data-stu-id="c699c-152">If exchanging, the total value of new purchase should be greater than $87.74</span></span>

<span data-ttu-id="c699c-153">**无法查看上一个计费周期的发票**</span><span class="sxs-lookup"><span data-stu-id="c699c-153">**Unable to see invoice for the last billing period**</span></span>

<span data-ttu-id="c699c-154">可能看不到发票的一些可能原因：</span><span class="sxs-lookup"><span data-stu-id="c699c-154">Some possible reasons you might not see an invoice:</span></span>

- <span data-ttu-id="c699c-155">订阅的每月信用额度未超过，或者有免费试用版。</span><span class="sxs-lookup"><span data-stu-id="c699c-155">You have a monthly credit amount with your subscription that you didn't exceed or you have a Free Trial.</span></span> <span data-ttu-id="c699c-156">仅当你付款时，才生成发票</span><span class="sxs-lookup"><span data-stu-id="c699c-156">An invoice is only generated when you owe money</span></span>
- <span data-ttu-id="c699c-157">订阅 Azure 的时间少于 30 天</span><span class="sxs-lookup"><span data-stu-id="c699c-157">It's less than 30 days from the day you subscribed to Azure</span></span>
- <span data-ttu-id="c699c-158">尚未生成发票。</span><span class="sxs-lookup"><span data-stu-id="c699c-158">The invoice isn't generated yet.</span></span> <span data-ttu-id="c699c-159">等待计费周期结束</span><span class="sxs-lookup"><span data-stu-id="c699c-159">Wait until the end of the billing period</span></span>
- <span data-ttu-id="c699c-160">如果你不是帐户管理员，则旧的发票可能不可用</span><span class="sxs-lookup"><span data-stu-id="c699c-160">If you're not the Account Administrator, older invoices may not be available to you</span></span>

<span data-ttu-id="c699c-161">**从 Azure 门户 (.pdf)**</span><span class="sxs-lookup"><span data-stu-id="c699c-161">**Download your invoice from Azure portal (.pdf)**</span></span>

- <span data-ttu-id="c699c-162">作为有权访问发票的用户，[](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)从 Azure 门户的订阅页面[选择订阅](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="c699c-162">Select your subscription from the [Subscriptions](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) page in Azure portal as [a user with access to invoices](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- <span data-ttu-id="c699c-163">选择 **发票**</span><span class="sxs-lookup"><span data-stu-id="c699c-163">Select **Invoices**</span></span>
- <span data-ttu-id="c699c-164">单击“**下载发票**”以查看 PDF 发票的副本。</span><span class="sxs-lookup"><span data-stu-id="c699c-164">Click **Download Invoice** to view a copy of your PDF invoice.</span></span> <span data-ttu-id="c699c-165">如果它表示 **不可用，** 请参阅为什么我看不到上一个计费周期 [的发票？](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)</span><span class="sxs-lookup"><span data-stu-id="c699c-165">If it says **Not available**, see [Why don't I see an invoice for the last billing period?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)</span></span>

<span data-ttu-id="c699c-166">**在电子邮件中接收发票 (.pdf)**</span><span class="sxs-lookup"><span data-stu-id="c699c-166">**Receive your invoice in email (.pdf)**</span></span>

- <span data-ttu-id="c699c-167">从订阅页面 [选择](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) 你的订阅。</span><span class="sxs-lookup"><span data-stu-id="c699c-167">Select your subscription from the [Subscriptions](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) page.</span></span> <span data-ttu-id="c699c-168">单击 **"发票"，** 然后"通过电子邮件发送我的发票"</span><span class="sxs-lookup"><span data-stu-id="c699c-168">Click **Invoices** then Email my invoice</span></span>
- <span data-ttu-id="c699c-169">单击 **"选择加入** "并接受条款。</span><span class="sxs-lookup"><span data-stu-id="c699c-169">Click **opt in** and accept the terms.</span></span> <span data-ttu-id="c699c-170">你必须选择加入你拥有的每个订阅</span><span class="sxs-lookup"><span data-stu-id="c699c-170">You will have to opt in for each subscription you own</span></span>

<span data-ttu-id="c699c-171">注意：如果按照步骤操作后没有收到电子邮件，请确保你的电子邮件地址在个人资料的通信首选项 [中是正确的](https://account.windowsazure.com/profile)</span><span class="sxs-lookup"><span data-stu-id="c699c-171">Note: If you don't get an email after following the steps, make sure your email address is correct in the [communication preferences on your profile](https://account.windowsazure.com/profile)</span></span>

<span data-ttu-id="c699c-172">**从 Azure 门户下载使用情况数据**</span><span class="sxs-lookup"><span data-stu-id="c699c-172">**Download your usage data from the Azure portal**</span></span>

- <span data-ttu-id="c699c-173">以帐户 [管理员角色登录到 Azure](https://account.windowsazure.com/Subscriptions) [帐户中心](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)</span><span class="sxs-lookup"><span data-stu-id="c699c-173">Sign into the [Azure Account Center](https://account.windowsazure.com/Subscriptions) as the [Account Admin](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)</span></span>
- <span data-ttu-id="c699c-174">选择要获取发票和使用情况信息的订阅</span><span class="sxs-lookup"><span data-stu-id="c699c-174">Select the subscription for which you want the invoice and usage information</span></span>
- <span data-ttu-id="c699c-175">选择 **帐单历史记录**</span><span class="sxs-lookup"><span data-stu-id="c699c-175">Select **Billing History**</span></span>
- <span data-ttu-id="c699c-176">选择 **"查看当前** 语句"以查看生成估计时的费用估计</span><span class="sxs-lookup"><span data-stu-id="c699c-176">Select **View Current Statement** to see an estimate of your charges at the time the estimate was generated</span></span>
- <span data-ttu-id="c699c-177">选择 **"下载** 使用情况"以将每日使用率数据下载为 CSV 文件。</span><span class="sxs-lookup"><span data-stu-id="c699c-177">Select **Download Usage** to download the daily usage data as a CSV file.</span></span> <span data-ttu-id="c699c-178">如果看到两个版本可用，请下载版本 2</span><span class="sxs-lookup"><span data-stu-id="c699c-178">If you see two versions available, download version 2</span></span>

<span data-ttu-id="c699c-179">其他问题： [访问预留实例文档](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="c699c-179">Other questions: [Visit reserved instance docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="c699c-180">**推荐文档**</span><span class="sxs-lookup"><span data-stu-id="c699c-180">**Recommended Documents**</span></span>

- [<span data-ttu-id="c699c-181">计费基础知识</span><span class="sxs-lookup"><span data-stu-id="c699c-181">Billing basics</span></span>](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="c699c-182">了解如何应用预留实例折扣</span><span class="sxs-lookup"><span data-stu-id="c699c-182">Understand how the Reserved Instance discount is applied</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="c699c-183">下载或查看 Azure 帐单发票和每日使用情况数据</span><span class="sxs-lookup"><span data-stu-id="c699c-183">Download or view your Azure billing invoice and daily usage data</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="c699c-184">了解如何应用预留实例折扣</span><span class="sxs-lookup"><span data-stu-id="c699c-184">Understand how the Reserved Instance discount is applied</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="c699c-185">了解"按时付费"订阅的预留实例使用情况</span><span class="sxs-lookup"><span data-stu-id="c699c-185">Understand Reserved Instance usage for your Pay-As-You-Go subscription</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="c699c-186">了解企业注册的预留实例使用情况</span><span class="sxs-lookup"><span data-stu-id="c699c-186">Understand Reserved Instance usage for your Enterprise enrollment</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="c699c-187">预留实例中不包括 Windows 软件成本</span><span class="sxs-lookup"><span data-stu-id="c699c-187">Windows software costs not included with Reserved instances</span></span>](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="c699c-188">合作伙伴中心云解决方案提供商云解决方案提供商计划 (云解决方案) 预留实例</span><span class="sxs-lookup"><span data-stu-id="c699c-188">Reserved Instances in Partner Central Cloud Solution Provider (CSP) program</span></span>](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)