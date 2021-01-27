---
title: 用户问题疑难解答
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886784"
---
# <a name="announcements"></a><span data-ttu-id="7ff2b-102">公告</span><span class="sxs-lookup"><span data-stu-id="7ff2b-102">Announcements</span></span>

<span data-ttu-id="7ff2b-103">关注 Google 关于测试兼容性的指南，测试你的应用受影响的情况。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-103">Follow Google's guidance on testing compatibility to test whether your apps are affected.</span></span> <span data-ttu-id="7ff2b-104">Google 的指南可以在 https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support 处找到。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-104">Google's guidance is available in https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support.</span></span>

<span data-ttu-id="7ff2b-105">确保在使用客户 Google 账户登陆用户时查看了系统的 Web 视图或系统浏览器。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-105">Ensure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="7ff2b-106">有关详细信息，请参阅[仅使用 Chrome 浏览器登陆应用的问题](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-106">For more information, see [Issues signing in to application(s) using Chrome browser only](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>


<span data-ttu-id="7ff2b-107">**我无法在我的 Azure AD 目录中创建新用户**</span><span class="sxs-lookup"><span data-stu-id="7ff2b-107">**I can't create a new user in my Azure AD directory**</span></span>

<span data-ttu-id="7ff2b-108">要解决无法在 Azure AD 中创建新用户的问题，执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="7ff2b-108">To troubleshoot the issue of not being able to create a new user in Azure AD, perform the following steps:</span></span>

1. <span data-ttu-id="7ff2b-109">确保你具有创建新的标准用户的权限。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="7ff2b-110">只有 Azure Active Directory (AD) 中的全局管理员或用户管理员角色可以创建新的标准用户。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-110">Only the global administrator or user administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="7ff2b-111">如果你不属于上述角色，需请求管理员将你添加到某个上述角色，或让他们为你创建新的用户账户。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
2. <span data-ttu-id="7ff2b-112">确保域中的用户名在你的 Azure AD 中完成过验证。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="7ff2b-113">如果你在 Azure AD 中没有任何验证过的自定义域名，你可以使用以 \*.onmicrosoft.com 结尾的 Azure AD 初始域名。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
3. <span data-ttu-id="7ff2b-114">确保用户名所在域不是从你的本地 AD 上与 Azure AD 联合的域。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="7ff2b-115">无法使用从本地联合的域名将用户添加到云。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
4. <span data-ttu-id="7ff2b-116">确保没有其他用户或联系人已经使用了你想要分配给新用户的用户名。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="7ff2b-117">用户名必须是 Azure AD 中唯一的。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-117">User names must be unique across Azure AD.</span></span>
5. <span data-ttu-id="7ff2b-118">参阅你的 Azure AD 的 [Azure AD 角色和管理员](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-118">See [Azure AD roles and administrators](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
6. <span data-ttu-id="7ff2b-119">参阅你的 Azure AD 的[域名](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains)。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-119">See the [domain names](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) for your Azure AD.</span></span>
7. <span data-ttu-id="7ff2b-120">检查 [审核日志](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) 来查看关于最近创建的或删除的用户的详细信息，比如谁执行的操作以及何时执行的。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-120">Review [Audit logs](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
8. <span data-ttu-id="7ff2b-121">有关添加新用户的详细信息，请参阅[使用 Azure 门户在 Azure AD 中创建新用户](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .</span></span>
9. <span data-ttu-id="7ff2b-122">有关 Azure AD 中管理员角色权限的详细信息，请参阅 [Azure AD 管理角色](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-122">For more information on administrator role permissions in Azure AD, see [Azure AD administrative roles](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).</span></span>
10. <span data-ttu-id="7ff2b-123">有关使用 Azure AD Powershell 创建用户的详细信息，请参阅[ Azure AD PowerShell 创建新用户](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser)。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-123">For details on creating a user using Azure AD Powershell, see [Azure AD PowerShell to create a new user](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).</span></span>

<span data-ttu-id="7ff2b-124">**自助注册问题**</span><span class="sxs-lookup"><span data-stu-id="7ff2b-124">**Problem with self-service sign up**</span></span>

<span data-ttu-id="7ff2b-125">要解决自助注册相关问题，执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="7ff2b-125">To troubleshoot issues regarding self-service sign up, perform the following steps:</span></span>

1. <span data-ttu-id="7ff2b-126">要通过应用使用自助注册，首先为你的租户启用自助注册。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-126">To use self-service sign-up with your applications, first enable self-service sign-up for your tenant.</span></span> 
2. <span data-ttu-id="7ff2b-127">要为应用启用支持自助注册，请将其添加到你的用户流中。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-127">To enable an application to support self-service sign up, add it to your user flow .</span></span> <span data-ttu-id="7ff2b-128">下一次转到应用的登陆页面时，你将会看到选项 \**_没有账户？现在创建！_* _.</span><span class="sxs-lookup"><span data-stu-id="7ff2b-128">The next time you go to the login page for that application, you'll see an option \**_No account? Create one!_* _.</span></span> <span data-ttu-id="7ff2b-129">然后自助注册过程将会开始。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-129">This starts the self-service sign-up process.</span></span>
3. <span data-ttu-id="7ff2b-130">有关如何使用自助注册在 Azure AD 上填充组织，请参阅 [Azure AD 自助注册](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup)。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-130">For information on how to use self-service sign up to populate an organization in Azure AD, see [Self-service sign up for Azure AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).</span></span>
4. <span data-ttu-id="7ff2b-131">一旦将用户流与一个或多个应用关联，访问该应用的用户就可以注册并使用在用户流中配置的选项获取来宾账户。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-131">Once you associate the user flow with one or more applications, users who visit that app will be able to sign up and gain a guest account using the options configured in the user flow.</span></span> <span data-ttu-id="7ff2b-132">有关注册和获取来宾账户的详细信息，用户可以参阅[来宾用户自助注册](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow)。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-132">For more information on signing up and gaining a guest account, the users can see [Self-service sign-up for guest users](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).</span></span>

<span data-ttu-id="7ff2b-133">_ *邀请外部用户的有关问题*\*</span><span class="sxs-lookup"><span data-stu-id="7ff2b-133">_ *Problem inviting an external user*\*</span></span>

<span data-ttu-id="7ff2b-134">要解决邀请外部用户的相关问题，执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="7ff2b-134">To troubleshoot issues regarding inviting an external user, perform the following step:</span></span>

<span data-ttu-id="7ff2b-135">确保你将用户邀请发送到了用户注册时使用的电子邮箱中。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-135">Ensure that you send a user's invitation to the email address that matches the name that the user signs in with.</span></span> <span data-ttu-id="7ff2b-136">如果你将邀请发送到用户的代理电子邮箱中，用户将无法进行兑换。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-136">If you send the invitation to a user's proxy email address, the user can't redeem it.</span></span> <span data-ttu-id="7ff2b-137">有关详细信息，请参阅 [Azure AD B2B 文档](https://docs.microsoft.com/azure/active-directory/external-identities/)。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-137">For more information, see [Azure AD B2B documentation](https://docs.microsoft.com/azure/active-directory/external-identities/).</span></span>

<span data-ttu-id="7ff2b-138">**我无法将许可证分配给用户**</span><span class="sxs-lookup"><span data-stu-id="7ff2b-138">**I can't assign licenses to a user**</span></span>

<span data-ttu-id="7ff2b-139">要解决给用户分配许可证的相关问题，执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="7ff2b-139">To troubleshoot issues regarding assigning licenses to a user, perform the following steps:</span></span>

1. <span data-ttu-id="7ff2b-140">要管理用户许可证，确保你使用的是下列的必需管理员角色账户: 全局管理员、许可证管理员或用户管理员。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-140">To manage user licenses, ensure that you use an account with one of the required administrator roles: global administrator, license administrator, or user administrator.</span></span> <span data-ttu-id="7ff2b-141">你可以在 **目录角色** 选项卡中查看用户的角色。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-141">You can check the user’s role in the **Directory role** tab on the user blade.</span></span>
2. <span data-ttu-id="7ff2b-142">如果你正在使用 Azure 门户且许可证分配发生故障，请单击右上角的通知按钮。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-142">If you are using the Azure portal and license assignment is failing, click the notification in the upper-right corner.</span></span> <span data-ttu-id="7ff2b-143">然后带有错误详细信息的边栏选项卡会打开。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-143">This opens a blade with details about what went wrong.</span></span> <span data-ttu-id="7ff2b-144">在大多数情况下，它提供了足够供你理解和解决问题的信息。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-144">In most cases that is enough to understand and resolve the problem.</span></span>
3. <span data-ttu-id="7ff2b-145">在完成用户许可证分配之前，确保已经为用户设置好 **使用位置** 属性。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-145">Before a license can be assigned to a user, ensure that the **Usage Location** property is set for the user.</span></span> <span data-ttu-id="7ff2b-146">通过查看用户边栏选项卡中的 **个人资料** 选项卡来验证用户的此属性已设置。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-146">Verify the user has that property set by viewing the **Profile** tab on the user blade.</span></span>
4. <span data-ttu-id="7ff2b-147">确保你将发放的许可证所属的产品有足够多可用的许可证。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-147">Ensure there are enough available licenses for the product you are trying to assign.</span></span> <span data-ttu-id="7ff2b-148">你可以在 Azure 门户的 [Azure Active Directory -> 许可证 -> 所有产品](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products)中查看可用的许可证数量。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-148">You can see the number of available licenses in the Azure portal, at [Azure Active Directory -> Licenses -> All products](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).</span></span>
5. <span data-ttu-id="7ff2b-149">用户可能已经有了会与你将发送给他们的许可证在服务上相冲突的别的许可证。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-149">The user may already have another license whose services conflict with those in the new license you are trying to assign.</span></span> <span data-ttu-id="7ff2b-150">比如，如果用户具有 Exchange Online（计划 1）服务，你将不能发送给他们 Exchange Online（计划 2）的许可证。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-150">For example, if the user has the Exchange Online (Plan 1) service enabled, you won’t be able to assign a license with the Exchange Online (Plan 2).</span></span> <span data-ttu-id="7ff2b-151">禁用正在使用的服务来发送新的许可证。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-151">Disable one of the services to allow the new license assignment.</span></span> <span data-ttu-id="7ff2b-152">如果你在使用 Azure 门户或 PowerShell cmdlets，**问题详细信息** 页面列出了造成冲突的具体服务。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-152">If you are using the Azure portal or PowerShell cmdlets, the **problem details** page lists the specific services that are causing the conflict.</span></span>
6. <span data-ttu-id="7ff2b-153">如果你想要删除发生故障的许可证，用户的其他许可服务可能是依赖于你将要删除的服务的。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-153">If you are trying to remove a license and that is failing, the user might have other licenses with services that depend on the services you are trying to remove.</span></span> <span data-ttu-id="7ff2b-154">如果你在使用 Azure 门户或 PowerShell cmdlets，错误信息将会列出了有依赖关系的具体服务。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-154">If you are using the Azure portal or PowerShell cmdlets, the error message will list the specific services that have dependencies.</span></span>
7. <span data-ttu-id="7ff2b-155">如果你想理解为什么某个许可证从用户处被添加/删除（例如，你组织中的谁做出了这样的更改），请查看审核日志。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-155">If you want to understand why a license was added/removed from a user (for example, who else in your organization may have made changes), check the audit logs.</span></span> <span data-ttu-id="7ff2b-156">将筛选器设置为 **许可证活动** 来显示所有的修改，包括执行操作的“主角”。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-156">Set the filter to **license activities** to show all modifications, including the "actor" that performed them.</span></span>
8. <span data-ttu-id="7ff2b-157">如果你在使用 Exchange Online，你的租户中的一些用户可能会通过相同的代理地址值被错误地配置。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-157">If you are using Exchange Online, some users in your tenant may be incorrectly configured with the same proxy address value.</span></span> <span data-ttu-id="7ff2b-158">在这种情况下，你可能会在许可证操作故障时看到一般错误消息。</span><span class="sxs-lookup"><span data-stu-id="7ff2b-158">In such cases, you may see generic error messages when a license operation fails.</span></span> <span data-ttu-id="7ff2b-159">[这篇文章](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used)包含关于此问题的详细信息，包括[如何使用远程 PowerShell 连接到 Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell) 的信息。要确认租户中的哪些用户包含相同的代理地址，请执行 Exchange Online cmdlet:</span><span class="sxs-lookup"><span data-stu-id="7ff2b-159">[This article](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) contains more information about this problem, including information on [how to connect to Exchange Online using remote PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).To identify which users in your tenant, contain the same proxy address, execute this Exchange Online cmdlet:</span></span>

<span data-ttu-id="7ff2b-160">运行</span><span class="sxs-lookup"><span data-stu-id="7ff2b-160">Run</span></span>

<span data-ttu-id="7ff2b-161">Get-Recipient | where {$_.EmailAddresses -match <user principal name>} | fL Name, RecipientType,emailaddresses</span><span class="sxs-lookup"><span data-stu-id="7ff2b-161">Get-Recipient | where {$_.EmailAddresses -match <user principal name>} | fL Name, RecipientType,emailaddresses</span></span>




