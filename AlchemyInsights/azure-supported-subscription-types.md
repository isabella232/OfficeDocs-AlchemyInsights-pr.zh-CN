---
title: 支持的订阅类型
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
- "6675"
ms.openlocfilehash: 46bc60435c3f8477e9f274d90c39d0f1c6a523c6
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791355"
---
# <a name="supported-subscription-types"></a><span data-ttu-id="7190d-102">支持的订阅类型</span><span class="sxs-lookup"><span data-stu-id="7190d-102">Supported subscription types</span></span>

<span data-ttu-id="7190d-103">请查看支持的订阅类型以继续操作。</span><span class="sxs-lookup"><span data-stu-id="7190d-103">Please review the supported subscription types to proceed further.</span></span>

[<span data-ttu-id="7190d-104">支持的订阅类型</span><span class="sxs-lookup"><span data-stu-id="7190d-104">Supported subscription types</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

<span data-ttu-id="7190d-105">**转移帐单所有权**</span><span class="sxs-lookup"><span data-stu-id="7190d-105">**Transfer billing ownership**</span></span>

<span data-ttu-id="7190d-106">将 Azure 门户用作需要转移订阅的帐单帐户的“[帐户管理员](https://ms.portal.azure.com/)”</span><span class="sxs-lookup"><span data-stu-id="7190d-106">Azure portal as the [Account Admin](https://ms.portal.azure.com/) of the billing account that has the subscription you want to transfer</span></span>

- <span data-ttu-id="7190d-107">在“ **成本管理 + 帐单** ”上搜索。</span><span class="sxs-lookup"><span data-stu-id="7190d-107">Search on **Cost Management + Billing** .</span></span> <span data-ttu-id="7190d-108">从左侧窗格选择 **“订阅”** 。</span><span class="sxs-lookup"><span data-stu-id="7190d-108">Select **Subscriptions** from left-pane.</span></span> <span data-ttu-id="7190d-109">你可能需要选择计费范围，然后再选择“ **订阅** ”或 “ **Azure 订阅** ”（具体取决于访问权限）。</span><span class="sxs-lookup"><span data-stu-id="7190d-109">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions** .</span></span>
- <span data-ttu-id="7190d-110">选择要转移的订阅的“转移帐单所有权”</span><span class="sxs-lookup"><span data-stu-id="7190d-110">Select Transfer billing ownership for the subscription you want to transfer</span></span>
- <span data-ttu-id="7190d-111">输入帐户的电子邮件地址，该帐户的用户是订阅的新所有者的帐单管理员，然后选择 **发送转移请求**</span><span class="sxs-lookup"><span data-stu-id="7190d-111">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="7190d-112">用户将收到一封电子邮件，其中包含检查转移请求的说明。</span><span class="sxs-lookup"><span data-stu-id="7190d-112">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="7190d-113">若要批准转移请求，用户可选择电子邮件中的链接，并按照说明进行操作。</span><span class="sxs-lookup"><span data-stu-id="7190d-113">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="7190d-114">注意：如果你将订阅的帐单所有权转移到另一个 Azure AD 租户中的用户帐户，则所有[基于角色的访问控制（RBAC）](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)以便在订阅中管理资源的权限将被永久删除。</span><span class="sxs-lookup"><span data-stu-id="7190d-114">Note: If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="7190d-115">只有新所有者才拥有在订阅中管理资源的权限。</span><span class="sxs-lookup"><span data-stu-id="7190d-115">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="7190d-116">有关详细信息，请参阅“[将订阅转移到另一个 Azure AD 租户中的用户](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)”。</span><span class="sxs-lookup"><span data-stu-id="7190d-116">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="7190d-117">**转移订阅的所有权**</span><span class="sxs-lookup"><span data-stu-id="7190d-117">**Transfer Ownership of Subscription**</span></span>

<span data-ttu-id="7190d-118">“订阅所有权转移”的先决条件是：用于管理订阅中的资源的基于角色的访问权限（RBAC）将失去访问权限。</span><span class="sxs-lookup"><span data-stu-id="7190d-118">Subscription Ownership Transfer prerequisites role based access (RBAC) to manage resources in the subscription lose their access.</span></span> <span data-ttu-id="7190d-119">有关将现有订阅添加到租户的详细信息，请参阅“[将 Azure 订阅关联或添加到 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)”。</span><span class="sxs-lookup"><span data-stu-id="7190d-119">For more information about adding an existing subscription to a tenant, see [Associate or add an Azure subscription to Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

- <span data-ttu-id="7190d-120">当前计费周期中包含现有未清金额的“订阅转移”将不会被转移到新帐户中的支付工具。</span><span class="sxs-lookup"><span data-stu-id="7190d-120">Subscription Transfer with an existing outstanding amount from the current billing cycle will not be transferred to the new payment instrument in the new account.</span></span> <span data-ttu-id="7190d-121">新帐户中的用户可用的唯一信息是上个月的订阅费用。</span><span class="sxs-lookup"><span data-stu-id="7190d-121">The only information available to the users in new account is the last month's cost for your subscription.</span></span> <span data-ttu-id="7190d-122">其他使用情况和帐单历史记录不会随订阅转移。</span><span class="sxs-lookup"><span data-stu-id="7190d-122">The rest of the usage and billing history does not transfer with the subscription.</span></span>
- <span data-ttu-id="7190d-123">仅在企业协议门户支持企业协议（EA）订阅的帐单所有权转移</span><span class="sxs-lookup"><span data-stu-id="7190d-123">Transfer billing ownership of Enterprise Agreement (EA) subscriptions is currently supported in the Enterprise Agreement Portal only</span></span>
- <span data-ttu-id="7190d-124">将面向信贷的订阅（如 Visual Studio、BizSpark、Microsoft 合作伙伴网络等）转移给新用户需要具有 Visual Studio/Microsoft 合作伙伴网络许可证以接受转移请求</span><span class="sxs-lookup"><span data-stu-id="7190d-124">Transferring a credit-oriented subscription like Visual Studio, BizSpark, Microsoft Partner Network to a new user requires to have a Visual Studio/Microsoft partner network license to accept the transfer request</span></span>
- <span data-ttu-id="7190d-125">所有资源（如虚拟机、磁盘和网站）均已成功转移到新帐户。</span><span class="sxs-lookup"><span data-stu-id="7190d-125">All resources like Virtual Machines, disks, and websites transfer to the new account successfully.</span></span> <span data-ttu-id="7190d-126">跨租户订阅转移中的以下资源可能会受到影响：</span><span class="sxs-lookup"><span data-stu-id="7190d-126">The following resources could be affected in a cross-tenant subscription transfer:</span></span>

<span data-ttu-id="7190d-127">**Azure AD 域服务**</span><span class="sxs-lookup"><span data-stu-id="7190d-127">**Azure AD Domain Services**</span></span>

<span data-ttu-id="7190d-128">密钥保管库</span><span class="sxs-lookup"><span data-stu-id="7190d-128">Azure Key Vaults</span></span>

- <span data-ttu-id="7190d-129">[SQL 相关用户和数据库](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support)可能会受到影响，尤其是当客户使用与 Azure Active Directory 相关的身份验证时</span><span class="sxs-lookup"><span data-stu-id="7190d-129">[SQL related users and databases](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) could be impacted, especially if the customer uses an Azure Active Directory related authentication</span></span>
- <span data-ttu-id="7190d-130">使用 Azure Active Directory 身份验证配置的 **应用服务** 可能会受到影响</span><span class="sxs-lookup"><span data-stu-id="7190d-130">**App Services** configured with Azure Active Directory authentication could be impacted</span></span>
- <span data-ttu-id="7190d-131">取消 Azure 订阅后，已连接至 Azure 订阅的 **Visual Studio Team** 服务帐户可能会暂时失去访问权限</span><span class="sxs-lookup"><span data-stu-id="7190d-131">**Visual Studio Team** Services accounts connected to Azure subscriptions may temporarily lose access when the connected Azure subscription is cancelled</span></span>

<span data-ttu-id="7190d-132">**推荐文档**</span><span class="sxs-lookup"><span data-stu-id="7190d-132">**Recommended Documents**</span></span>

<span data-ttu-id="7190d-133">接受帐单所有权后的步骤：</span><span class="sxs-lookup"><span data-stu-id="7190d-133">Steps after accepting billing ownership:</span></span>

- <span data-ttu-id="7190d-134">若要保留帐单所有权，但想要更改订阅类型，请参阅：“[将 Azure 订阅切换到其他优惠](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)”</span><span class="sxs-lookup"><span data-stu-id="7190d-134">To retain billing ownership, but change the type of your subscription, refer: [Switch your Azure subscription to another offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- [<span data-ttu-id="7190d-135">转移 Visual Studio、Microsoft 合作伙伴网络（MPN）和即付即用开发/测试订阅</span><span class="sxs-lookup"><span data-stu-id="7190d-135">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="7190d-136">转移企业协议（EA）订阅的帐单所有权</span><span class="sxs-lookup"><span data-stu-id="7190d-136">Transfer billing ownership of Enterprise Agreement (EA) subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)
- [<span data-ttu-id="7190d-137">转移所有权常见问题</span><span class="sxs-lookup"><span data-stu-id="7190d-137">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="7190d-138">有关转移所有权问题的疑难解答</span><span class="sxs-lookup"><span data-stu-id="7190d-138">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)