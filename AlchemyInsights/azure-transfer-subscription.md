---
title: 转移 Azure 账单所有权
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: 74b7cc879973790b7532106c80b718856682a334
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755537"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="bddb2-102">转移 Azure 账单所有权</span><span class="sxs-lookup"><span data-stu-id="bddb2-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="bddb2-103">以拥有你想要转移的订阅的帐单帐户管理员身份登录到 [Azure 门户](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="bddb2-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="bddb2-104">如果不确定你是否为管理员，或如果需要确定谁是管理员，请参阅[确认帐户帐单管理员](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)。</span><span class="sxs-lookup"><span data-stu-id="bddb2-104">If you're not sure if you're an administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

1. <span data-ttu-id="bddb2-105">搜索“_成本管理 + 帐单_”。</span><span class="sxs-lookup"><span data-stu-id="bddb2-105">Search for _Cost Management + Billing_.</span></span>
1. <span data-ttu-id="bddb2-106">从左侧窗格选择“**订阅**”。</span><span class="sxs-lookup"><span data-stu-id="bddb2-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="bddb2-107">根据访问权限，可能需要选择计费范围，然后再选择 **订阅** 或 **Azure 订阅**。</span><span class="sxs-lookup"><span data-stu-id="bddb2-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
1. <span data-ttu-id="bddb2-108">选择要转移的订阅的 **转移帐单所有权**。</span><span class="sxs-lookup"><span data-stu-id="bddb2-108">Select **Transfer billing ownership** for the subscription you want to transfer.</span></span>
1. <span data-ttu-id="bddb2-109">输入帐户的电子邮件地址，该帐户的用户将为订阅的新所有者的帐单管理员，然后选择 **发送转移请求**。</span><span class="sxs-lookup"><span data-stu-id="bddb2-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**.</span></span>
1. <span data-ttu-id="bddb2-110">用户将收到一封电子邮件，其中包含检查转移请求的说明。</span><span class="sxs-lookup"><span data-stu-id="bddb2-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="bddb2-111">若要批准转移请求，用户可选择电子邮件中的链接，并按照说明进行操作。</span><span class="sxs-lookup"><span data-stu-id="bddb2-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="bddb2-112">请注意，如果你将订阅的帐单所有权转移到另一个 Azure AD 租户中的用户帐户，则将永久删除用于管理订阅中资源的所有[基于角色的访问控制（RBAC）](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)分配。</span><span class="sxs-lookup"><span data-stu-id="bddb2-112">Please note that if you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="bddb2-113">仅新的所有者才拥有在订阅中管理资源的权限。</span><span class="sxs-lookup"><span data-stu-id="bddb2-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="bddb2-114">有关如何为订阅更改目录的更多信息，请参见[将订阅转移到另一个 Azure AD 租户中的用户](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="bddb2-114">For more information about how to change directory for a subscription, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="bddb2-115">_**对发票的重要影响：**_ 如果已转让 Azure 订阅的帐单所有权，则费用将按比例分配。</span><span class="sxs-lookup"><span data-stu-id="bddb2-115">_**Important impact on your invoices**_: if you've transferred billing ownership for an Azure subscription, your charges will be pro-rated.</span></span> <span data-ttu-id="bddb2-116">你将能够按照以下方式访问发票：</span><span class="sxs-lookup"><span data-stu-id="bddb2-116">You'll be able to access the invoices as per the following:</span></span>  

1. <span data-ttu-id="bddb2-117">从  Azure 门户中的 [订阅页面中](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)选择你的订阅，作为 [可以访问发票的用户](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)，然后选择 **发票**。</span><span class="sxs-lookup"><span data-stu-id="bddb2-117">Select your subscription from the [Subscriptions page](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) in the Azure portal as [a user with access to invoices](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support), then select **Invoices**.</span></span>
1. <span data-ttu-id="bddb2-118">点击 **下载发票** 以查看 PDF 发票副本。</span><span class="sxs-lookup"><span data-stu-id="bddb2-118">Click **Download Invoice** to view a copy of your PDF invoice.</span></span> <span data-ttu-id="bddb2-119">如果显示 _不可用_，请参阅 [为何无法查看上次帐单周期的发票？](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)。</span><span class="sxs-lookup"><span data-stu-id="bddb2-119">If it says _Not available_, see [Why don't I see an invoice for the last billing period?](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice).</span></span>
1. <span data-ttu-id="bddb2-120">你还可通过点击 **帐单周期** 来查看每日使用量，以获取发票的 PDF 格式和详细的每日使用量文件的副本 (.CSV)。</span><span class="sxs-lookup"><span data-stu-id="bddb2-120">You can also view your daily usage by clicking the **billing period** to obtain a PDF of your invoice and a copy of your detailed daily usage file (.CSV).</span></span> <span data-ttu-id="bddb2-121">有关更多信息，请参阅 [获取发票和使用情况数据](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="bddb2-121">For more information, see [Get invoice and usage data](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="bddb2-122">**推荐文档**</span><span class="sxs-lookup"><span data-stu-id="bddb2-122">**Recommended Documents**</span></span>

- [<span data-ttu-id="bddb2-123">将 Azure 订阅的帐单所有权转移到其他帐户</span><span class="sxs-lookup"><span data-stu-id="bddb2-123">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="bddb2-124">关于转移 Azure 订阅的帐单所有权</span><span class="sxs-lookup"><span data-stu-id="bddb2-124">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="bddb2-125">转移 Visual Studio、Microsoft 合作伙伴网络（MPN）和即付即用开发/测试订阅</span><span class="sxs-lookup"><span data-stu-id="bddb2-125">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="bddb2-126">转移所有权常见问题</span><span class="sxs-lookup"><span data-stu-id="bddb2-126">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="bddb2-127">有关转移所有权问题的疑难解答</span><span class="sxs-lookup"><span data-stu-id="bddb2-127">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
