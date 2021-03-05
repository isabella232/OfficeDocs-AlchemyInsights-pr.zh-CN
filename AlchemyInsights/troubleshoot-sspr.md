---
title: SSPR 疑难解答
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428570"
---
# <a name="troubleshoot-sspr"></a><span data-ttu-id="60c0d-102">SSPR 疑难解答</span><span class="sxs-lookup"><span data-stu-id="60c0d-102">Troubleshoot SSPR</span></span>

<span data-ttu-id="60c0d-103">**配置密码重置时遇到问题**</span><span class="sxs-lookup"><span data-stu-id="60c0d-103">**I'm having trouble configuring password reset**</span></span>

- <span data-ttu-id="60c0d-104">如果你是管理员，并且正在查找如何启用自助服务密码重置，请参阅教程"启用 [SSPR"，](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)为组织配置密码重置。</span><span class="sxs-lookup"><span data-stu-id="60c0d-104">If you are administrator and looking for how to enable self-service password reset, see [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization.</span></span> <span data-ttu-id="60c0d-105">你可能还需要查看 [许可要求](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="60c0d-105">You may also want to review the [licensing requirements](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span> <span data-ttu-id="60c0d-106">您必须在组织中分配至少一个许可证。</span><span class="sxs-lookup"><span data-stu-id="60c0d-106">You must have at least one license assigned in your organization.</span></span>
    - <span data-ttu-id="60c0d-107">**仅云用户** - 任何 Office 365 (O365) 付费 SKU 或 Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="60c0d-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="60c0d-108">**云和/或** 本地用户 - Azure AD Premium P1 或 P2、企业移动性 + 安全性 (EMS) 或安全生产企业 (SPE) </span><span class="sxs-lookup"><span data-stu-id="60c0d-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
- <span data-ttu-id="60c0d-109">有关自助服务密码重置的其他问题，请查看 [我们的常见问题解答](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="60c0d-109">For additional questions about self-service password reset, review [our FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="60c0d-110">**我收到错误消息**</span><span class="sxs-lookup"><span data-stu-id="60c0d-110">**I'm getting an error message**</span></span>

<span data-ttu-id="60c0d-111">查看本文以查找常见错误及其解决方案 [：自助密码重置疑难解答](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="60c0d-111">Review this article to find common errors and their solutions: [Troubleshoot self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="60c0d-112">**密码重置策略有问题**</span><span class="sxs-lookup"><span data-stu-id="60c0d-112">**I'm having a problem with my password reset policy**</span></span>

- <span data-ttu-id="60c0d-113">如果密码重置策略未如预期方式运行，或者对密码重置策略有疑问，请查看本文 [：Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)中的密码策略和限制。</span><span class="sxs-lookup"><span data-stu-id="60c0d-113">If your password reset policy is not behaving as expected, or if you have questions about password reset policies, review this article: [Password policies and restrictions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="60c0d-114">密码重置策略不适用于管理员。</span><span class="sxs-lookup"><span data-stu-id="60c0d-114">Password reset policies do not apply to administrators.</span></span> <span data-ttu-id="60c0d-115">Microsoft 对任意 Azure 管理员角色强制执行强默认双门密码重置策略。</span><span class="sxs-lookup"><span data-stu-id="60c0d-115">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role.</span></span> <span data-ttu-id="60c0d-116">确保您正在与不是管理员的用户一起进行测试。</span><span class="sxs-lookup"><span data-stu-id="60c0d-116">Make sure that you are testing with a user who is not an administrator.</span></span> <span data-ttu-id="60c0d-117">有关管理员重置策略详细信息，请参阅本文： [管理员重置策略差异](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)。</span><span class="sxs-lookup"><span data-stu-id="60c0d-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span></span>

<span data-ttu-id="60c0d-118">**我不想我的用户注册密码重置的其他安全信息**</span><span class="sxs-lookup"><span data-stu-id="60c0d-118">**I don't want my users to register additional security info for password reset**</span></span>

<span data-ttu-id="60c0d-119">可以使用 API、 (或 Azure AD Connect 为) 预填充电子邮件和电话属性的数据。</span><span class="sxs-lookup"><span data-stu-id="60c0d-119">You can pre-populate data (email and phone attributes) for your users using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="60c0d-120">若要了解如何阅读：</span><span class="sxs-lookup"><span data-stu-id="60c0d-120">To learn how read:</span></span>

- [<span data-ttu-id="60c0d-121">在不要求用户注册的情况下部署密码重置</span><span class="sxs-lookup"><span data-stu-id="60c0d-121">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [<span data-ttu-id="60c0d-122">密码重置使用的数据</span><span class="sxs-lookup"><span data-stu-id="60c0d-122">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="60c0d-123">**我希望用户注册其他安全信息以重置密码**</span><span class="sxs-lookup"><span data-stu-id="60c0d-123">**I want my users to register their additional security info for password reset**</span></span>

1. <span data-ttu-id="60c0d-124">让用户通过引导他们注册其安全信息以重置自助服务[密码aka.ms/ssprsetup。](https://mysignins.microsoft.com/security-info)</span><span class="sxs-lookup"><span data-stu-id="60c0d-124">Have your users register their security info for self service password reset by directing them to [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span></span>
1. <span data-ttu-id="60c0d-125">在用户或管理员 (填充用户密码后) ，将用户aka.ms/sspr以便用户能够重置自己的密码。 [](https://passwordreset.microsoftonline.com/)</span><span class="sxs-lookup"><span data-stu-id="60c0d-125">After data is populated for the user (by the user or by the admin), direct your user to [aka.ms/sspr](https://passwordreset.microsoftonline.com/) so your users can be empowered to reset their own passwords.</span></span>
1. <span data-ttu-id="60c0d-126">如果用户仍遇到问题，他们很可能是联合用户或密码 **哈希同步** 用户。</span><span class="sxs-lookup"><span data-stu-id="60c0d-126">If users are still experiencing problems they are most likely **federated** or **password hash synched** users.</span></span> <span data-ttu-id="60c0d-127">这意味着密码写回服务可能存在问题。</span><span class="sxs-lookup"><span data-stu-id="60c0d-127">This means there is likely a problem with the Password Writeback service.</span></span>