---
title: 重置密码时出现问题
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2021
ms.locfileid: "50585648"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="b8164-102">重置密码时出现问题</span><span class="sxs-lookup"><span data-stu-id="b8164-102">Problems resetting password</span></span>

<span data-ttu-id="b8164-103">以下是在重置密码和可能的解决方案时可能面临的一些问题：</span><span class="sxs-lookup"><span data-stu-id="b8164-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="b8164-104">**我遇到密码重置未涵盖在其他类别中的问题**</span><span class="sxs-lookup"><span data-stu-id="b8164-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="b8164-105">确保你有权重置密码。</span><span class="sxs-lookup"><span data-stu-id="b8164-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="b8164-106">只有全局、密码和用户管理员可以重置用户密码。</span><span class="sxs-lookup"><span data-stu-id="b8164-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="b8164-107">全局管理员还可以重置其他特权管理员的密码。</span><span class="sxs-lookup"><span data-stu-id="b8164-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="b8164-108">确保您了解许可要求：</span><span class="sxs-lookup"><span data-stu-id="b8164-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="b8164-109">必须在组织中分配至少一个许可证</span><span class="sxs-lookup"><span data-stu-id="b8164-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="b8164-110">仅云用户 - 任何 Office 365 (O365) 付费 SKU 或 Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="b8164-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="b8164-111">云和/或本地用户 - Azure AD Premium P1 或 P2、企业移动性 + 安全性 (EMS) 或安全生产企业 (SPE) </span><span class="sxs-lookup"><span data-stu-id="b8164-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="b8164-112">若要阅读有关许可要求的信息，请参阅文章 [Azure AD 自助服务密码重置的许可要求](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="b8164-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="b8164-113">**测试我设置的密码重置策略时遇到问题**</span><span class="sxs-lookup"><span data-stu-id="b8164-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="b8164-114">最近应用的策略可能需要几分钟才能跨所有数据中心和终点进行复制。</span><span class="sxs-lookup"><span data-stu-id="b8164-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="b8164-115">与数据中心的物理距离也会影响更改应用速度。</span><span class="sxs-lookup"><span data-stu-id="b8164-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="b8164-116">使用最终用户（而不是管理员）进行测试，然后通过一小组用户进行试点。</span><span class="sxs-lookup"><span data-stu-id="b8164-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="b8164-117">Azure 门户中配置的策略仅适用于最终用户，不适用于管理员。</span><span class="sxs-lookup"><span data-stu-id="b8164-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="b8164-118">Microsoft 对 Azure 管理员角色强制执行强默认双门密码重置策略 (例如：全局管理员、支持管理员、密码管理员等) </span><span class="sxs-lookup"><span data-stu-id="b8164-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="b8164-119">了解有关管理员 [策略的更多信息](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)。</span><span class="sxs-lookup"><span data-stu-id="b8164-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="b8164-120">**我想要部署密码重置，但不希望我的用户注册其他安全信息**</span><span class="sxs-lookup"><span data-stu-id="b8164-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="b8164-121">为用户预填充数据，以便他们不必这样做！</span><span class="sxs-lookup"><span data-stu-id="b8164-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="b8164-122">- 作为管理员，可以在向组织推出密码重置之前为用户设置电话和电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="b8164-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="b8164-123">可以使用 API、PowerShell 或 Azure AD Connect 进行此操作。</span><span class="sxs-lookup"><span data-stu-id="b8164-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="b8164-124">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="b8164-124">More information here:</span></span>
- [<span data-ttu-id="b8164-125">无需用户注册即可部署密码重置</span><span class="sxs-lookup"><span data-stu-id="b8164-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="b8164-126">密码重置使用的数据</span><span class="sxs-lookup"><span data-stu-id="b8164-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="b8164-127">**密码重置按钮灰出**</span><span class="sxs-lookup"><span data-stu-id="b8164-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="b8164-128">你无权重置此用户的密码。</span><span class="sxs-lookup"><span data-stu-id="b8164-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="b8164-129">只有全局、密码和用户管理员可以重置用户密码。</span><span class="sxs-lookup"><span data-stu-id="b8164-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="b8164-130">全局管理员还可以重置其他特权管理员的密码。</span><span class="sxs-lookup"><span data-stu-id="b8164-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="b8164-131">**我看不到密码重置边栏选项卡**</span><span class="sxs-lookup"><span data-stu-id="b8164-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="b8164-132">你无权重置密码。</span><span class="sxs-lookup"><span data-stu-id="b8164-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="b8164-133">只有全局、密码和用户管理员可以重置用户密码。</span><span class="sxs-lookup"><span data-stu-id="b8164-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="b8164-134">全局管理员还可以重置其他特权管理员的密码。</span><span class="sxs-lookup"><span data-stu-id="b8164-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="b8164-135">**在密码重置中看不到本地集成边栏选项卡**</span><span class="sxs-lookup"><span data-stu-id="b8164-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="b8164-136">本地集成边栏选项卡仅在混合环境中显示 - 这意味着你正在使用密码写回操作本地用户的密码。</span><span class="sxs-lookup"><span data-stu-id="b8164-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="b8164-137">如果：</span><span class="sxs-lookup"><span data-stu-id="b8164-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="b8164-138">您没有使用密码写回</span><span class="sxs-lookup"><span data-stu-id="b8164-138">You are not using password writeback</span></span>
    - <span data-ttu-id="b8164-139">密码写回的安装/连接存在问题</span><span class="sxs-lookup"><span data-stu-id="b8164-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="b8164-140">Azure AD Connect 的安装/连接存在问题</span><span class="sxs-lookup"><span data-stu-id="b8164-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="b8164-141">有关密码写回问题的更多疑难解答步骤，请参阅"密码写回疑 [难解答"部分](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="b8164-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="b8164-142">**不知道如何重置用户密码**</span><span class="sxs-lookup"><span data-stu-id="b8164-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="b8164-143">以适当的管理员登录 Azure 门户。</span><span class="sxs-lookup"><span data-stu-id="b8164-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="b8164-144">转到"用户和组"边栏选项卡，选择 **"所有用户"。**</span><span class="sxs-lookup"><span data-stu-id="b8164-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="b8164-145">从列表中选择用户。</span><span class="sxs-lookup"><span data-stu-id="b8164-145">Select a user from the list.</span></span>
1. <span data-ttu-id="b8164-146">对于所选用户，选择 **"概述**"，然后在命令栏中单击"**重置密码"。**</span><span class="sxs-lookup"><span data-stu-id="b8164-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="b8164-147">按照屏幕上的说明进行操作。</span><span class="sxs-lookup"><span data-stu-id="b8164-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="b8164-148">仅通过 Azure 门户执行的重置支持密码写回。</span><span class="sxs-lookup"><span data-stu-id="b8164-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="b8164-149">**我在 Office 365 管理门户或 Office 365 移动应用程序中重置本地用户密码，但用户仍无法登录**</span><span class="sxs-lookup"><span data-stu-id="b8164-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="b8164-150">此门户不支持密码写回。</span><span class="sxs-lookup"><span data-stu-id="b8164-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="b8164-151">在 Azure 门户中再次重置用户密码 - portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="b8164-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

