---
title: 启用成本管理
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599053"
---
# <a name="enable-cost-management"></a><span data-ttu-id="b5bbd-102">启用成本管理</span><span class="sxs-lookup"><span data-stu-id="b5bbd-102">Enable cost management</span></span>

<span data-ttu-id="b5bbd-103">**为您的组织禁用的成本是什么意思？**</span><span class="sxs-lookup"><span data-stu-id="b5bbd-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="b5bbd-104">使用 Enterprise 协议 (EA) 或 Microsoft Customer 协议 (MCA) 帐户的组织可以禁用对成本信息和定价信息的访问。</span><span class="sxs-lookup"><span data-stu-id="b5bbd-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="b5bbd-105">登录到 Azure 门户后，他们可以使用计费 Api 以编程方式获取发票 (一旦选择了) 和使用详细信息。</span><span class="sxs-lookup"><span data-stu-id="b5bbd-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="b5bbd-106">**如何允许其他用户访问发票**</span><span class="sxs-lookup"><span data-stu-id="b5bbd-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="b5bbd-107">转到 Azure 门户中的 " **订阅" 边栏** 。</span><span class="sxs-lookup"><span data-stu-id="b5bbd-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="b5bbd-108">选择 " **发票** "，然后 **访问发票**。</span><span class="sxs-lookup"><span data-stu-id="b5bbd-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="b5bbd-109">打开访问权限，然后保存更改，以允许订阅范围的角色中的用户下载发票。</span><span class="sxs-lookup"><span data-stu-id="b5bbd-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="b5bbd-110">帐户管理员还可以将配置为通过电子邮件发送发票。</span><span class="sxs-lookup"><span data-stu-id="b5bbd-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="b5bbd-111">若要了解详细信息，请参阅 [在电子邮件中获取发票](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)。</span><span class="sxs-lookup"><span data-stu-id="b5bbd-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="b5bbd-112">**如何将用户添加到帐单阅读者角色**</span><span class="sxs-lookup"><span data-stu-id="b5bbd-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="b5bbd-113">转到 Azure 门户中的 " **订阅" 边栏** 。</span><span class="sxs-lookup"><span data-stu-id="b5bbd-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="b5bbd-114">选择 " **(IAM) 的" 访问控制** "，然后单击" **添加**"。</span><span class="sxs-lookup"><span data-stu-id="b5bbd-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="b5bbd-115">在 "**选择角色**" 页中选择 "**帐单阅读** 者"。</span><span class="sxs-lookup"><span data-stu-id="b5bbd-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="b5bbd-116">键入要邀请的用户的电子邮件，然后单击 **"确定"** 以发送邀请。</span><span class="sxs-lookup"><span data-stu-id="b5bbd-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="b5bbd-117">按照邀请电子邮件中提供的说明，以付费阅读者的形式登录。</span><span class="sxs-lookup"><span data-stu-id="b5bbd-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="b5bbd-118">有关详细信息，请参阅 [授予对帐单的访问权限](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)。</span><span class="sxs-lookup"><span data-stu-id="b5bbd-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="b5bbd-119">**推荐的文档**</span><span class="sxs-lookup"><span data-stu-id="b5bbd-119">**Recommended documents**</span></span>

- [<span data-ttu-id="b5bbd-120">通过 EA 门户启用 DA 和 AO 视图</span><span class="sxs-lookup"><span data-stu-id="b5bbd-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="b5bbd-121">成本管理中包括的成本</span><span class="sxs-lookup"><span data-stu-id="b5bbd-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="b5bbd-122">支持的 Microsoft Azure 提供</span><span class="sxs-lookup"><span data-stu-id="b5bbd-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="b5bbd-123">查看成本分析中的成本</span><span class="sxs-lookup"><span data-stu-id="b5bbd-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="b5bbd-124">提供对帐单信息的访问权限</span><span class="sxs-lookup"><span data-stu-id="b5bbd-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="b5bbd-125">检查 Microsoft 客户协议的访问权限</span><span class="sxs-lookup"><span data-stu-id="b5bbd-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






