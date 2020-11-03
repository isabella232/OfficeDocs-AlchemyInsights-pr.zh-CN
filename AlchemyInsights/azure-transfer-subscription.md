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
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840581"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="7eed7-102">转移 Azure 账单所有权</span><span class="sxs-lookup"><span data-stu-id="7eed7-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="7eed7-103">以帐单帐户的管理员身份登录到 [Azure 门户](https://portal.azure.com/)（该帐单帐户拥有你想要转移的订阅）。</span><span class="sxs-lookup"><span data-stu-id="7eed7-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="7eed7-104">如果不确定你是否是管理员，或需要确定谁才是管理员，请参阅“[确认帐户帐单管理员](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)”。</span><span class="sxs-lookup"><span data-stu-id="7eed7-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="7eed7-105">在“ **成本管理 + 帐单** ”上搜索。</span><span class="sxs-lookup"><span data-stu-id="7eed7-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="7eed7-106">从左侧窗格选择“ **订阅** ”。</span><span class="sxs-lookup"><span data-stu-id="7eed7-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="7eed7-107">你可能需要选择计费范围，然后再选择“ **订阅** ”或 “ **Azure 订阅** ”（具体取决于访问权限）。</span><span class="sxs-lookup"><span data-stu-id="7eed7-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="7eed7-108">选择要转移的订阅的“ **转移帐单所有权** ”</span><span class="sxs-lookup"><span data-stu-id="7eed7-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="7eed7-109">输入帐户的电子邮件地址，该帐户的用户是订阅的新所有者的帐单管理员，然后选择 **发送转移请求**</span><span class="sxs-lookup"><span data-stu-id="7eed7-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="7eed7-110">用户将收到一封电子邮件，其中包含检查转移请求的说明。</span><span class="sxs-lookup"><span data-stu-id="7eed7-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="7eed7-111">若要批准转移请求，用户可选择电子邮件中的链接，并按照说明进行操作。</span><span class="sxs-lookup"><span data-stu-id="7eed7-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="7eed7-112">**注意** ：如果你将订阅的帐单所有权转移到另一个 Azure AD 租户中的用户帐户，则所有[基于角色的访问控制（RBAC）](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)以便在订阅中管理资源的权限将被永久删除。</span><span class="sxs-lookup"><span data-stu-id="7eed7-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="7eed7-113">只有新所有者才拥有在订阅中管理资源的权限。</span><span class="sxs-lookup"><span data-stu-id="7eed7-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="7eed7-114">有关详细信息，请参阅“[将订阅转移到另一个 Azure AD 租户中的用户](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)”。</span><span class="sxs-lookup"><span data-stu-id="7eed7-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="7eed7-115">**推荐文档**</span><span class="sxs-lookup"><span data-stu-id="7eed7-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="7eed7-116">将 Azure 订阅的帐单所有权转移到其他帐户</span><span class="sxs-lookup"><span data-stu-id="7eed7-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="7eed7-117">关于转移 Azure 订阅的帐单所有权</span><span class="sxs-lookup"><span data-stu-id="7eed7-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="7eed7-118">转移 Visual Studio、Microsoft 合作伙伴网络（MPN）和即付即用开发/测试订阅</span><span class="sxs-lookup"><span data-stu-id="7eed7-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="7eed7-119">转移所有权常见问题</span><span class="sxs-lookup"><span data-stu-id="7eed7-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="7eed7-120">有关转移所有权问题的疑难解答</span><span class="sxs-lookup"><span data-stu-id="7eed7-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
