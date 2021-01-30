---
title: 凭据问题
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052943"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="2cb5b-102">凭据问题</span><span class="sxs-lookup"><span data-stu-id="2cb5b-102">Issues with credentials</span></span>

<span data-ttu-id="2cb5b-103">[Microsoft 标识平台和 OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 客户端凭据流描述如何直接针对 OAuth 2.0 客户端凭据授予流进行编程。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="2cb5b-104">**如何管理应用程序的密码或证书凭据？**</span><span class="sxs-lookup"><span data-stu-id="2cb5b-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="2cb5b-105">在 Azure CLI 中，可以使用 [az 广告](https://docs.microsoft.com/cli/azure/ad/app/credential) 应用凭据删除、列出或重置应用程序的密码或证书凭据。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="2cb5b-106">**我的用户如何重置其密码？**</span><span class="sxs-lookup"><span data-stu-id="2cb5b-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="2cb5b-107">用户需要 [先注册自助服务密码重置](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) ，然后才能重置其密码。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="2cb5b-108">用户注册后，可以按照本文中的说明重置其密码：重置 [工作或学校密码](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="2cb5b-109">**我的用户如何更改其密码？**</span><span class="sxs-lookup"><span data-stu-id="2cb5b-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="2cb5b-110">用户可以按照本文中的步骤更改其密码： [如何更改密码](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="2cb5b-111">他们还可以 [管理应用密码进行两步验证](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="2cb5b-112">**我的用户在更改或重置密码时收到错误**</span><span class="sxs-lookup"><span data-stu-id="2cb5b-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="2cb5b-113">此链接将提供有关用户尝试重置其密码时可能出现的常见问题的信息：常见问题 [及其解决方案](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="2cb5b-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="2cb5b-114">**重置用户密码时遇到问题**</span><span class="sxs-lookup"><span data-stu-id="2cb5b-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="2cb5b-115">请确保你有权重置密码。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="2cb5b-116">*只有全局、密码和用户管理员可以重置用户密码。*</span><span class="sxs-lookup"><span data-stu-id="2cb5b-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="2cb5b-117">全局管理员还可以重置其他特权管理员的密码。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="2cb5b-118">确保您了解许可要求：</span><span class="sxs-lookup"><span data-stu-id="2cb5b-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="2cb5b-119">必须在组织中分配至少一个许可证：</span><span class="sxs-lookup"><span data-stu-id="2cb5b-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="2cb5b-120">**仅云用户** - 任何 Office 365 (O365) 付费 SKU 或 Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="2cb5b-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="2cb5b-121">**云和/或** 本地用户 - Azure AD Premium P1 或 P2、企业移动性 + 安全性 (EMS) 或 Secure Productive Enterprise (SPE) </span><span class="sxs-lookup"><span data-stu-id="2cb5b-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="2cb5b-122">若要了解有关许可要求的信息，请参阅 [Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)自助服务密码重置的许可要求。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="2cb5b-123">若要重置用户密码，在 Azure AD 中查找用户。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="2cb5b-124">然后，在该用户的概述边栏选项卡上，单击"重置密码"按钮。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="2cb5b-125">**密码重置按钮灰出**</span><span class="sxs-lookup"><span data-stu-id="2cb5b-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="2cb5b-126">您 **无权重置此** 用户的密码。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="2cb5b-127">*只有全局、密码和用户管理员可以重置用户密码。*</span><span class="sxs-lookup"><span data-stu-id="2cb5b-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="2cb5b-128">全局管理员还可以重置其他特权管理员的密码。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="2cb5b-129">**我看不到密码重置边栏选项卡**</span><span class="sxs-lookup"><span data-stu-id="2cb5b-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="2cb5b-130">您无权重置密码。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="2cb5b-131">*只有全局、密码和用户管理员可以重置用户密码。*</span><span class="sxs-lookup"><span data-stu-id="2cb5b-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="2cb5b-132">全局管理员还可以重置其他特权管理员的密码。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="2cb5b-133">**在密码重置中看不到本地集成边栏选项卡**</span><span class="sxs-lookup"><span data-stu-id="2cb5b-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="2cb5b-134">本地集成边栏选项卡仅出现在混合环境中 - 这意味着你正在使用密码写回操作本地用户的密码。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="2cb5b-135">如果：</span><span class="sxs-lookup"><span data-stu-id="2cb5b-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="2cb5b-136">您没有使用密码写回</span><span class="sxs-lookup"><span data-stu-id="2cb5b-136">You are not using password writeback</span></span>
  - <span data-ttu-id="2cb5b-137">密码写回的安装/连接存在问题</span><span class="sxs-lookup"><span data-stu-id="2cb5b-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="2cb5b-138">Azure AD Connect 的安装/连接存在问题</span><span class="sxs-lookup"><span data-stu-id="2cb5b-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="2cb5b-139">有关密码写回问题的更多疑难解答步骤，请参阅 [密码写回疑难解答](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="2cb5b-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="2cb5b-140">**不知道如何重置用户密码**</span><span class="sxs-lookup"><span data-stu-id="2cb5b-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="2cb5b-141">以适当的管理员登录 Azure 门户。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="2cb5b-142">转到"**用户和组"** 边栏选项卡，选择 **"所有用户"。**</span><span class="sxs-lookup"><span data-stu-id="2cb5b-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="2cb5b-143">从列表中选择用户。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-143">Select a user from the list.</span></span>
4. <span data-ttu-id="2cb5b-144">对于所选用户，选择 **"概述**"，然后在命令栏中，选择"**重置密码"。**</span><span class="sxs-lookup"><span data-stu-id="2cb5b-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="2cb5b-145">选择 **"重置密码"** 按钮并按照屏幕上的说明操作。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="2cb5b-146">仅通过 Azure 门户执行的 **重置** 支持密码写回。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="2cb5b-147">**我在 Office 365 管理门户或 Office 365 移动应用程序中重置本地用户的密码，但该用户仍无法登录**</span><span class="sxs-lookup"><span data-stu-id="2cb5b-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="2cb5b-148">此门户不支持密码写回。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="2cb5b-149">在 Azure 门户中再次重置用户密码。</span><span class="sxs-lookup"><span data-stu-id="2cb5b-149">Reset the user's password again in the Azure portal.</span></span>
