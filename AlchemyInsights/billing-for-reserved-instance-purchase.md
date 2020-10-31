---
title: 预留实例购买账单
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
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/30/2020
ms.locfileid: "48815980"
---
# <a name="billing-for-reserved-instance-purchase"></a><span data-ttu-id="a4305-102">预留实例购买账单</span><span class="sxs-lookup"><span data-stu-id="a4305-102">Billing for Reserved Instance purchase</span></span>

<span data-ttu-id="a4305-103">预留实例购买将按照与您在购买时选择的订阅相关的付款方式进行收费。</span><span class="sxs-lookup"><span data-stu-id="a4305-103">The reserved instance purchase is charged to the payment method tied to the subscription that you select at the time of purchase.</span></span> <span data-ttu-id="a4305-104">订阅类型必须是企业协议（优惠号码： MS-CHAP，AZR-0017P）、即用即付支付（优惠号码： MS-CHAP-AZR-0003P）、Microsoft 客户协议或 CSP。</span><span class="sxs-lookup"><span data-stu-id="a4305-104">The subscription type must be an enterprise agreement (offer number: MS-AZR-0017P), Pay-As-You-Go (offer number: MS-AZR-0003P), Microsoft Customer Agreement or CSP.</span></span>

- <span data-ttu-id="a4305-105">对于企业订阅，费用从注册的货币承诺余额中扣除或作为超额收费</span><span class="sxs-lookup"><span data-stu-id="a4305-105">For an enterprise subscription, the charges are deducted from the enrollment's monetary commitment balance or charged as overage</span></span>
- <span data-ttu-id="a4305-106">对于即用即付订阅，收费通过订阅上的信用卡或发票付款方式计费</span><span class="sxs-lookup"><span data-stu-id="a4305-106">For Pay-As-You-Go subscription, the charges are billed to the credit card or invoice payment method on the subscription</span></span>

<span data-ttu-id="a4305-107">**取消保留**</span><span class="sxs-lookup"><span data-stu-id="a4305-107">**Cancelling Reservation**</span></span>

- <span data-ttu-id="a4305-108">**自助服务：** 可自行使用 [Azure 门户](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)取消或更换保留实例。</span><span class="sxs-lookup"><span data-stu-id="a4305-108">**Self-service:** You can cancel or exchange a reserved instance yourself using [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade).</span></span> <span data-ttu-id="a4305-109">选择保留，然后单击退款或交换。</span><span class="sxs-lookup"><span data-stu-id="a4305-109">Select the reservation and click on refund or exchange.</span></span> <span data-ttu-id="a4305-110">请注意，你必须持有“保留订单”的所有者访问权限才能进行交换或退款。</span><span class="sxs-lookup"><span data-stu-id="a4305-110">Note that you must have owner access on the Reservation Order to exchange or refund.</span></span> <span data-ttu-id="a4305-111">仅持有对“保留”的访问权限将不允许你进行退款或交换。</span><span class="sxs-lookup"><span data-stu-id="a4305-111">Access to only the Reservation will not let you proceed with refund or exchange.</span></span> <span data-ttu-id="a4305-112">请求“保留订单”所有者授予你对“保留订单”的访问权限</span><span class="sxs-lookup"><span data-stu-id="a4305-112">Ask the Reservation Order owner to give you owner access to the Reservation Order</span></span>
- <span data-ttu-id="a4305-113">**交换策略：** 你可以与同一类型的另一保留进行交换，交换保留将 **不收到处罚** 。</span><span class="sxs-lookup"><span data-stu-id="a4305-113">**Exchange policy:** You can exchange a reservation for another reservation of the same type – there are **no penalties** on reservation exchange.</span></span> <span data-ttu-id="a4305-114">新保留的整体承诺应大于已交换保留的退款金额与未来的每月付款（如果适用）</span><span class="sxs-lookup"><span data-stu-id="a4305-114">The total commitment with new reservation should be greater than the sum of exchanged reservation’s refund amount and the future monthly payments (if applicable)</span></span>
- <span data-ttu-id="a4305-115">**退款政策：** 退款总额和已取消的未来付款情况在长达 12 个月的滚动窗口内不得超过 $50,000 美元。</span><span class="sxs-lookup"><span data-stu-id="a4305-115">**Refund policy:** Sum of refund and the cancelled future payments cannot exceed $50,000 USD in a 12-month rolling window.</span></span> <span data-ttu-id="a4305-116">对于退款，我们 **目前不实施任何处罚收费** ，但可能在未来的退款中对其计费</span><span class="sxs-lookup"><span data-stu-id="a4305-116">We are **currently not charging any penalty** on refunds but could charge it on future refunds</span></span>

<span data-ttu-id="a4305-117">**例外：** 自助服务交换和取消功能不适用于美国政府企业协议客户</span><span class="sxs-lookup"><span data-stu-id="a4305-117">**Exceptions:** Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers</span></span>

- <span data-ttu-id="a4305-118">**API / PS / CLI** 支持不可用于取消和退款 [针对 Azure 保留的自助服务交换和退款](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="a4305-118">**API / PS / CLI** support is not available for cancellation and refunds [Self-service exchanges and refunds for Azure Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- <span data-ttu-id="a4305-119">自助服务交换和取消功能不可用于美国政府企业协议客户。</span><span class="sxs-lookup"><span data-stu-id="a4305-119">Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers.</span></span> <span data-ttu-id="a4305-120">支持其他美国政府订阅类型（包括“即付即用”和 CSP）</span><span class="sxs-lookup"><span data-stu-id="a4305-120">Other US Government subscription types including Pay-As-You-Go and CSP are supported</span></span>

<span data-ttu-id="a4305-121">了解详细信息： [如何处理退货和 exchange 事务](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) 了解详细信息： [exchange 和退款策略](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) 其他问题： [访问保留实例文档](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="a4305-121">Learn more : [How return and exchange transactions are processed](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Learn more : [Exchange and Refund policies](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Other questions: [Visit reserved instance docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="a4305-122">**交换现有保留实例（自助服务）**</span><span class="sxs-lookup"><span data-stu-id="a4305-122">**Exchange an existing reserved instance (Self-service)**</span></span>

<span data-ttu-id="a4305-123">可将现有保留与同一类型的另一保留进行交换。</span><span class="sxs-lookup"><span data-stu-id="a4305-123">You can exchange a reservation for another reservation of the same type.</span></span> <span data-ttu-id="a4305-124">如果不再需要保留，你也可以退款，每年最高 $50,000 美元。</span><span class="sxs-lookup"><span data-stu-id="a4305-124">You can also refund a reservation, up to $50,000 USD per year, if you no longer need it.</span></span> <span data-ttu-id="a4305-125">自助服务交换和取消功能不可用于美国政府企业协议客户。</span><span class="sxs-lookup"><span data-stu-id="a4305-125">Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers.</span></span> <span data-ttu-id="a4305-126">支持其他美国政府订阅类型（包括“即付即用”和 CSP）。</span><span class="sxs-lookup"><span data-stu-id="a4305-126">Other US Government subscription types including Pay-As-You-Go and CSP are supported.</span></span> <span data-ttu-id="a4305-127">你必须持有“保留订单”的所有者访问权限才能对现有保留进行交换或退款。</span><span class="sxs-lookup"><span data-stu-id="a4305-127">You must have owner access on the Reservation Order to exchange or refund an existing reservation.</span></span>

<span data-ttu-id="a4305-128">以下步骤将提供完成事务的指导过程</span><span class="sxs-lookup"><span data-stu-id="a4305-128">The following steps will guide on the procedure to complete the transaction</span></span>

<span data-ttu-id="a4305-129">1. 登录到 [Azure 门户](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)。</span><span class="sxs-lookup"><span data-stu-id="a4305-129">1.Log in to your [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade).</span></span> <span data-ttu-id="a4305-130">选择要退款的保留，然后单击 " **Exchange** 2"。选择要购买的虚拟机产品并键入数量。</span><span class="sxs-lookup"><span data-stu-id="a4305-130">Select the reservations that you want to refund and click **Exchange** 2.Select the VM product that you want to purchase and type a quantity.</span></span> <span data-ttu-id="a4305-131">在购买之前，请确保新的采购总额大于返回总数 [确定正确的大小](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)。</span><span class="sxs-lookup"><span data-stu-id="a4305-131">Make sure that the new purchase total is more than the return total [Determine the right size before you purchase](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).</span></span>
<span data-ttu-id="a4305-132">3. 查看并完成事务</span><span class="sxs-lookup"><span data-stu-id="a4305-132">3.Review and complete the transaction</span></span>

<span data-ttu-id="a4305-133">**保留实例的退款**</span><span class="sxs-lookup"><span data-stu-id="a4305-133">**Refund for a reserved instance**</span></span>

<span data-ttu-id="a4305-134">若要退款保留，请转到“ **保留详细信息** ”，然后单击“ **退款** ”</span><span class="sxs-lookup"><span data-stu-id="a4305-134">To refund a reservation, go to **Reservation Details** and click **Refund**</span></span>

<span data-ttu-id="a4305-135">**按照比例的退款：**</span><span class="sxs-lookup"><span data-stu-id="a4305-135">**Pro-rated refund:**</span></span>

<span data-ttu-id="a4305-136">**用于退款和 exchange 的 ration 和最低要求示例** 前期保留示例：</span><span class="sxs-lookup"><span data-stu-id="a4305-136">**Pro-ration and minimum requirement examples for refund and exchange** Upfront reservation example:</span></span>

- <span data-ttu-id="a4305-137">你在 1 月 1 日花费 $120 购买了为期一年的 R1</span><span class="sxs-lookup"><span data-stu-id="a4305-137">You purchase a one-year term RI for $120 on January 1</span></span>
- <span data-ttu-id="a4305-138">在 4 月 7 日，你希望退款或交换此保留</span><span class="sxs-lookup"><span data-stu-id="a4305-138">On April 7th you want to refund or exchange this reservation</span></span>
- <span data-ttu-id="a4305-139">由于保留已活跃 97 天，你将获得 (1-97/365) \* $120 的退款。</span><span class="sxs-lookup"><span data-stu-id="a4305-139">Since the reservation has been live for 97 days, you will get (1-97/365) \* $120 back.</span></span> <span data-ttu-id="a4305-140">（即 $88.1）。</span><span class="sxs-lookup"><span data-stu-id="a4305-140">(i.e. $88.1).</span></span> <span data-ttu-id="a4305-141">目前没有退款处罚</span><span class="sxs-lookup"><span data-stu-id="a4305-141">There is currently no penalty on refunds</span></span>
- <span data-ttu-id="a4305-142">如果要交换，新的购买应高于 $88.1</span><span class="sxs-lookup"><span data-stu-id="a4305-142">If exchanging, your new purchase should be greater than $88.1</span></span>
- <span data-ttu-id="a4305-143">目前退款不会受到处罚</span><span class="sxs-lookup"><span data-stu-id="a4305-143">There is no penalty on refunds currently</span></span>

<span data-ttu-id="a4305-144">**计费套餐保留示例：**</span><span class="sxs-lookup"><span data-stu-id="a4305-144">**Billing plan reservation example:**</span></span>

- <span data-ttu-id="a4305-145">你购买了为期一年的 RI（每月支付 $10）</span><span class="sxs-lookup"><span data-stu-id="a4305-145">You purchase a one-year term RI for $10 per month</span></span>
- <span data-ttu-id="a4305-146">在 4 月 7 日，你希望退款或交换此保留</span><span class="sxs-lookup"><span data-stu-id="a4305-146">On April 7th you want to refund or exchange this reservation</span></span>
- <span data-ttu-id="a4305-147">由于上次的付款发生在 7 天前，你将获得 (1-7/31) \* $10 的退款。</span><span class="sxs-lookup"><span data-stu-id="a4305-147">Since the last payment happened 7 days, you will get (1-7/31) \* $10 back.</span></span> <span data-ttu-id="a4305-148">（即 $7.74）</span><span class="sxs-lookup"><span data-stu-id="a4305-148">(i.e. $7.74)</span></span>
- <span data-ttu-id="a4305-149">所取消的未来付款是 $80。</span><span class="sxs-lookup"><span data-stu-id="a4305-149">The future payments cancelled are $ 80.</span></span> <span data-ttu-id="a4305-150">目前没有退款处罚</span><span class="sxs-lookup"><span data-stu-id="a4305-150">There is currently no penalty on refunds</span></span>
- <span data-ttu-id="a4305-151">此取消将从你的 $50,000 退款限度中扣除 $87.74</span><span class="sxs-lookup"><span data-stu-id="a4305-151">This cancellation will deduct $87.74 from you’re the $50,000 refund limit</span></span>
- <span data-ttu-id="a4305-152">如果进行交换，则新购买的总额应大于 $87.74</span><span class="sxs-lookup"><span data-stu-id="a4305-152">If exchanging, the total value of new purchase should be greater than $87.74</span></span>

<span data-ttu-id="a4305-153">**无法查看上一付款期的发票**</span><span class="sxs-lookup"><span data-stu-id="a4305-153">**Unable to see invoice for the last billing period**</span></span>

<span data-ttu-id="a4305-154">您可能看不到发票的一些可能原因：</span><span class="sxs-lookup"><span data-stu-id="a4305-154">Some possible reasons you might not see an invoice:</span></span>

- <span data-ttu-id="a4305-155">你的订阅的月贷方金额与你的订阅不超过或你有免费试用版。</span><span class="sxs-lookup"><span data-stu-id="a4305-155">You have a monthly credit amount with your subscription that you didn't exceed or you have a Free Trial.</span></span> <span data-ttu-id="a4305-156">仅在欠资金时生成发票</span><span class="sxs-lookup"><span data-stu-id="a4305-156">An invoice is only generated when you owe money</span></span>
- <span data-ttu-id="a4305-157">从你的 Azure 订阅之日起的时间不到30天</span><span class="sxs-lookup"><span data-stu-id="a4305-157">It's less than 30 days from the day you subscribed to Azure</span></span>
- <span data-ttu-id="a4305-158">尚未生成发票。</span><span class="sxs-lookup"><span data-stu-id="a4305-158">The invoice isn't generated yet.</span></span> <span data-ttu-id="a4305-159">等到付款期结束</span><span class="sxs-lookup"><span data-stu-id="a4305-159">Wait until the end of the billing period</span></span>
- <span data-ttu-id="a4305-160">如果你不是帐户管理员，则可能无法使用较旧的发票</span><span class="sxs-lookup"><span data-stu-id="a4305-160">If you're not the Account Administrator, older invoices may not be available to you</span></span>

<span data-ttu-id="a4305-161">**从 Azure 门户下载你的发票 ( .pdf)**</span><span class="sxs-lookup"><span data-stu-id="a4305-161">**Download your invoice from Azure portal (.pdf)**</span></span>

- <span data-ttu-id="a4305-162">从 Azure 门户的 " [订阅](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) " 页中选择你的订阅作为 [具有发票访问权限的用户](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="a4305-162">Select your subscription from the [Subscriptions](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) page in Azure portal as [a user with access to invoices](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- <span data-ttu-id="a4305-163">选择 **发票**</span><span class="sxs-lookup"><span data-stu-id="a4305-163">Select **Invoices**</span></span>
- <span data-ttu-id="a4305-164">单击 " **下载发票** " 以查看 PDF 发票的副本。</span><span class="sxs-lookup"><span data-stu-id="a4305-164">Click **Download Invoice** to view a copy of your PDF invoice.</span></span> <span data-ttu-id="a4305-165">如果它指出 **不可用** ，请参阅 [为什么我在最后一次付款期内看不到发票？](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)</span><span class="sxs-lookup"><span data-stu-id="a4305-165">If it says **Not available** , see [Why don't I see an invoice for the last billing period?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)</span></span>

<span data-ttu-id="a4305-166">**通过电子邮件 ( .pdf) 接收你的发票**</span><span class="sxs-lookup"><span data-stu-id="a4305-166">**Receive your invoice in email (.pdf)**</span></span>

- <span data-ttu-id="a4305-167">从 " [订阅](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) " 页中选择订阅。</span><span class="sxs-lookup"><span data-stu-id="a4305-167">Select your subscription from the [Subscriptions](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) page.</span></span> <span data-ttu-id="a4305-168">单击 " **发票** " 然后通过电子邮件发送我的发票</span><span class="sxs-lookup"><span data-stu-id="a4305-168">Click **Invoices** then Email my invoice</span></span>
- <span data-ttu-id="a4305-169">单击 " **选择"** 并接受条款。</span><span class="sxs-lookup"><span data-stu-id="a4305-169">Click **opt in** and accept the terms.</span></span> <span data-ttu-id="a4305-170">您必须为自己拥有的每个订阅选择加入</span><span class="sxs-lookup"><span data-stu-id="a4305-170">You will have to opt in for each subscription you own</span></span>

<span data-ttu-id="a4305-171">注意：如果按照这些步骤操作后未收到电子邮件，请确保你的电子邮件地址在[你的个人资料的通信首选项](https://account.windowsazure.com/profile)中是正确的</span><span class="sxs-lookup"><span data-stu-id="a4305-171">Note: If you don't get an email after following the steps, make sure your email address is correct in the [communication preferences on your profile](https://account.windowsazure.com/profile)</span></span>

<span data-ttu-id="a4305-172">**从 Azure 门户下载你的使用情况数据**</span><span class="sxs-lookup"><span data-stu-id="a4305-172">**Download your usage data from the Azure portal**</span></span>

- <span data-ttu-id="a4305-173">以[帐户管理员](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)的身份登录[Azure 帐户中心](https://account.windowsazure.com/Subscriptions)</span><span class="sxs-lookup"><span data-stu-id="a4305-173">Sign into the [Azure Account Center](https://account.windowsazure.com/Subscriptions) as the [Account Admin](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)</span></span>
- <span data-ttu-id="a4305-174">选择要获取其发票和使用情况信息的订阅</span><span class="sxs-lookup"><span data-stu-id="a4305-174">Select the subscription for which you want the invoice and usage information</span></span>
- <span data-ttu-id="a4305-175">选择 **帐单历史记录**</span><span class="sxs-lookup"><span data-stu-id="a4305-175">Select **Billing History**</span></span>
- <span data-ttu-id="a4305-176">选择 " **查看当前报表** " 以查看估计生成估计时的费用估计值</span><span class="sxs-lookup"><span data-stu-id="a4305-176">Select **View Current Statement** to see an estimate of your charges at the time the estimate was generated</span></span>
- <span data-ttu-id="a4305-177">选择 " **下载使用率** " 以将每日使用率数据下载为 CSV 文件。</span><span class="sxs-lookup"><span data-stu-id="a4305-177">Select **Download Usage** to download the daily usage data as a CSV file.</span></span> <span data-ttu-id="a4305-178">如果看到可用的两个版本，请下载版本2</span><span class="sxs-lookup"><span data-stu-id="a4305-178">If you see two versions available, download version 2</span></span>

<span data-ttu-id="a4305-179">其他问题：[访问保留的实例文档](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="a4305-179">Other questions: [Visit reserved instance docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="a4305-180">**推荐文档**</span><span class="sxs-lookup"><span data-stu-id="a4305-180">**Recommended Documents**</span></span>

- [<span data-ttu-id="a4305-181">帐单基础知识</span><span class="sxs-lookup"><span data-stu-id="a4305-181">Billing basics</span></span>](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a4305-182">了解如何应用保留的实例折扣</span><span class="sxs-lookup"><span data-stu-id="a4305-182">Understand how the Reserved Instance discount is applied</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a4305-183">下载或查看你的 Azure 计费发票和日常使用情况数据</span><span class="sxs-lookup"><span data-stu-id="a4305-183">Download or view your Azure billing invoice and daily usage data</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a4305-184">了解如何应用保留的实例折扣</span><span class="sxs-lookup"><span data-stu-id="a4305-184">Understand how the Reserved Instance discount is applied</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a4305-185">了解随转到即用订阅的保留实例用法</span><span class="sxs-lookup"><span data-stu-id="a4305-185">Understand Reserved Instance usage for your Pay-As-You-Go subscription</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a4305-186">了解企业注册的保留实例用法</span><span class="sxs-lookup"><span data-stu-id="a4305-186">Understand Reserved Instance usage for your Enterprise enrollment</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a4305-187">保留实例不包含的 Windows 软件成本</span><span class="sxs-lookup"><span data-stu-id="a4305-187">Windows software costs not included with Reserved instances</span></span>](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a4305-188">合作伙伴中心云解决方案提供商 (CSP) 程序中的保留实例</span><span class="sxs-lookup"><span data-stu-id="a4305-188">Reserved Instances in Partner Central Cloud Solution Provider (CSP) program</span></span>](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)