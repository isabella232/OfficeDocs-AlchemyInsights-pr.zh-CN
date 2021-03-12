---
title: 解决组问题
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
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "50716103"
---
# <a name="troubleshoot-group-issues"></a><span data-ttu-id="56b87-102">解决组问题</span><span class="sxs-lookup"><span data-stu-id="56b87-102">Troubleshoot group issues</span></span>

<span data-ttu-id="56b87-103">**我需要将组分配给 Azure AD 角色**</span><span class="sxs-lookup"><span data-stu-id="56b87-103">**I need to assign a group to an Azure AD role**</span></span>

<span data-ttu-id="56b87-104">若要将 Azure Active Directory （AD） 组分配给 Azure AD 角色，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="56b87-104">To assign an Azure Active Directory (AD) group to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="56b87-105">创建新组 - 以创建新组：</span><span class="sxs-lookup"><span data-stu-id="56b87-105">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="56b87-106">a.</span><span class="sxs-lookup"><span data-stu-id="56b87-106">a.</span></span> <span data-ttu-id="56b87-107">使用特权角色管理员或全局管理员权限登录 Azure AD 管理中心。</span><span class="sxs-lookup"><span data-stu-id="56b87-107">Sign in to the Azure AD admin center with privileged role administrator or global administrator permissions.</span></span> 
    <span data-ttu-id="56b87-108">b.</span><span class="sxs-lookup"><span data-stu-id="56b87-108">b.</span></span> <span data-ttu-id="56b87-109">选择 Azure Active Directory >"组">"所有组">"新建组"。</span><span class="sxs-lookup"><span data-stu-id="56b87-109">Select Azure Active Directory > Groups > All groups > New group.</span></span> 
    <span data-ttu-id="56b87-110">c.</span><span class="sxs-lookup"><span data-stu-id="56b87-110">c.</span></span> <span data-ttu-id="56b87-111">创建组。</span><span class="sxs-lookup"><span data-stu-id="56b87-111">Create the group.</span></span>

2. <span data-ttu-id="56b87-112">在组创建期间或在组创建之后将角色分配给组。</span><span class="sxs-lookup"><span data-stu-id="56b87-112">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="56b87-113">a.</span><span class="sxs-lookup"><span data-stu-id="56b87-113">a.</span></span> <span data-ttu-id="56b87-114">要在创建组时将角色分配给组，请打开可以将 Azure AD 角色分配给组切换按钮，并创建组。</span><span class="sxs-lookup"><span data-stu-id="56b87-114">To assign a role to the group at the time of group creation, switch on the toggle Azure AD roles can be assigned to the group and create the group.</span></span>
    <span data-ttu-id="56b87-115">b.</span><span class="sxs-lookup"><span data-stu-id="56b87-115">b.</span></span> <span data-ttu-id="56b87-116">要在组创建后将角色分配给该组，请导航到新创建的组的“已分配角色”选项卡，然后将角色分配给该组。</span><span class="sxs-lookup"><span data-stu-id="56b87-116">To assign a role to the group after it has been created, navigate to the Assigned roles tab for the newly created group, and assign the role to the group.</span></span>

<span data-ttu-id="56b87-117">**我需要管理分配给 Azure AD 角色的组的成员身份**</span><span class="sxs-lookup"><span data-stu-id="56b87-117">**I need to manage membership of a group that is assigned to Azure AD role**</span></span>

1. <span data-ttu-id="56b87-118">为防止提升权限，默认情况下，只有特权角色管理员和全局管理员才能修改分配给角色的组的会员资格。</span><span class="sxs-lookup"><span data-stu-id="56b87-118">To prevent elevation of privileges, by default, only privileged role administrator and global administrator can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="56b87-119">但是，他们可以选择为这样的组分配所有者并委派此任务。</span><span class="sxs-lookup"><span data-stu-id="56b87-119">They can, however, choose to assign an owner for such a group and delegate this task.</span></span> <span data-ttu-id="56b87-120">有关详细信息，请参阅 [组在 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)。</span><span class="sxs-lookup"><span data-stu-id="56b87-120">For more information see, [Use cloud groups to manage role assignments in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span>
2. <span data-ttu-id="56b87-121">有关在 Azure AD 中向组分配角色的常见问题和疑难解答提示，请参阅 [分配给云组的角色的疑难](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)。</span><span class="sxs-lookup"><span data-stu-id="56b87-121">For common questions and troubleshooting tips for assigning roles to groups in Azure AD, see [Troubleshooting roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>

<span data-ttu-id="56b87-122">**动态组**</span><span class="sxs-lookup"><span data-stu-id="56b87-122">**Dynamic groups**</span></span>

1. <span data-ttu-id="56b87-123">如果找不到内置用户属性，请确保属性位于支持的属性列表中。</span><span class="sxs-lookup"><span data-stu-id="56b87-123">If you cannot find the built-in user attributes, ensure that the attribute is in the list of supported properties.</span></span>
2. <span data-ttu-id="56b87-124">如果要查找内置设备属性，请确保该属性位于设备属性列表中</span><span class="sxs-lookup"><span data-stu-id="56b87-124">If you are looking for built-in device attributes, ensure that the attribute is in the list of device attributes</span></span> 
3. <span data-ttu-id="56b87-125">除了内置的用户和设备属性，还可使用"扩展 [属性](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties)。</span><span class="sxs-lookup"><span data-stu-id="56b87-125">In addition to the built-in user and device attributes, you could also use [Extension Attributes](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties).</span></span> <span data-ttu-id="56b87-126">从本地 Windows Server AD 或连接的 SaaS 应用程序同步扩展属性后，属性应显示在规则生成器的下拉列表中。</span><span class="sxs-lookup"><span data-stu-id="56b87-126">After syncing extension attributes from on-premises Windows Server AD or from a connected SaaS application, the attributes should be visible in the drop-down list of the rule builder.</span></span> <span data-ttu-id="56b87-127">通过使用 PowerShell 查询用户属性并搜索属性名称，可在目录中找到自定义属性名称。</span><span class="sxs-lookup"><span data-stu-id="56b87-127">The custom attribute name can be found in the directory by querying a user's attribute using PowerShell and searching for the attribute name.</span></span> <span data-ttu-id="56b87-128">在规则语法中构建规则时，也可使用这些规则。</span><span class="sxs-lookup"><span data-stu-id="56b87-128">These could also be used when constructing rules in the rule syntax.</span></span>
4. <span data-ttu-id="56b87-129">确保租户具有相应的许可证。</span><span class="sxs-lookup"><span data-stu-id="56b87-129">Ensure that your tenant has the appropriate license.</span></span> <span data-ttu-id="56b87-130">动态组需要租户拥有 Azure AD P1 Premium 许可证。</span><span class="sxs-lookup"><span data-stu-id="56b87-130">Dynamic groups require the tenant to have an Azure AD P1 Premium license.</span></span> <span data-ttu-id="56b87-131">可在此处访问 Azure AD 许可证计划 [列表](https://azure.microsoft.com/pricing/details/active-directory/)。</span><span class="sxs-lookup"><span data-stu-id="56b87-131">The list of Azure AD license plans can be accessed [here](https://azure.microsoft.com/pricing/details/active-directory/).</span></span> <span data-ttu-id="56b87-132">可在此处访问企业移动性 + 安全性 [许可](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)。</span><span class="sxs-lookup"><span data-stu-id="56b87-132">Enterprise Mobility + Security licensing plans can be accessed [here](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing).</span></span>
5. <span data-ttu-id="56b87-133">确保创建动态组的用户的角色是全局管理员、Intune 管理员、组管理员或用户管理员。</span><span class="sxs-lookup"><span data-stu-id="56b87-133">Ensure that the role of the user creating the dynamic group is a global administrator, intune administrator, group administrator, or a user administrator.</span></span>
6. <span data-ttu-id="56b87-134">请留出一些时间，以便组进行填充。</span><span class="sxs-lookup"><span data-stu-id="56b87-134">Please allow time for the group to populate.</span></span> <span data-ttu-id="56b87-135">根据租户的大小，首次填充或规则更改后，组可能需要多达 24 小时进行填充。</span><span class="sxs-lookup"><span data-stu-id="56b87-135">Depending on the size of your tenant, the group may take up to 24 hours for populating for the first time or after a rule change.</span></span>
7. <span data-ttu-id="56b87-136">有关详细信息，请参阅 [动态组成员身份列表创建基于属性的规则](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)。</span><span class="sxs-lookup"><span data-stu-id="56b87-136">For more information, see [Create attribute-based rules for dynamic group membership](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).</span></span>

<span data-ttu-id="56b87-137">**我需要删除组**</span><span class="sxs-lookup"><span data-stu-id="56b87-137">**I need to delete a group**</span></span>

1. <span data-ttu-id="56b87-138">可以使用 Azure AD Powershell 模块中的 Remove-AzureADGroup cmdlet 从目录中删除组。</span><span class="sxs-lookup"><span data-stu-id="56b87-138">Groups can be deleted from the directory using the Remove-AzureADGroup cmdlet in the Azure AD Powershell module.</span></span>
2. <span data-ttu-id="56b87-139">在 Azure AD 中尝试删除同步组之前，请确保已删除所有已分配的许可证以避免错误。</span><span class="sxs-lookup"><span data-stu-id="56b87-139">Before attempting to delete a synced group in Azure AD, ensure you have deleted all assigned licenses  to avoid errors.</span></span>
3. <span data-ttu-id="56b87-140">有关删除组的信息，请参阅 [已分配许可证的组时删除](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)。</span><span class="sxs-lookup"><span data-stu-id="56b87-140">For more information on deleting groups, see [Deleting a group with an assigned license](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).</span></span>

<span data-ttu-id="56b87-141">**我需要还原已删除的组**</span><span class="sxs-lookup"><span data-stu-id="56b87-141">**I need to restore a deleted group**</span></span>

1. <span data-ttu-id="56b87-142">如果删除了 Office 365 组，则只能在永久删除前 30 天将其还原。</span><span class="sxs-lookup"><span data-stu-id="56b87-142">If an Office 365 group is deleted, it can only be restored up to 30 days before permanent deletion occurs.</span></span> <span data-ttu-id="56b87-143">永久删除后，无法再还原组。</span><span class="sxs-lookup"><span data-stu-id="56b87-143">Once permanently deleted, the group can no longer be restored.</span></span> <span data-ttu-id="56b87-144">在[此处](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)了解有关还原组。</span><span class="sxs-lookup"><span data-stu-id="56b87-144">Learn more about restoring groups [here](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>
2. <span data-ttu-id="56b87-145">安全组和通讯组不支持此功能。</span><span class="sxs-lookup"><span data-stu-id="56b87-145">This functionality is not supported for security groups and distribution groups.</span></span>
3. <span data-ttu-id="56b87-146">确保你有权还原 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="56b87-146">Ensure you are authorized to restore an Office 365 group.</span></span> <span data-ttu-id="56b87-147">全局管理员、组管理员、用户帐户管理员、Intune 服务管理员、合作伙伴第 1 层或第 2 层支持以及组的所有者能够还原组。</span><span class="sxs-lookup"><span data-stu-id="56b87-147">Global administrators, group administrators, user account administrators, intune service administrators, partner tier1 or tier2 support, and the owner of the group can be able to restore a group.</span></span>
4. <span data-ttu-id="56b87-148">删除和还原动态组时，它被视为新组，然后根据规则进行填充。</span><span class="sxs-lookup"><span data-stu-id="56b87-148">When a dynamic group is deleted and restored, it is seen as a new group and re-populated according to the rule.</span></span> <span data-ttu-id="56b87-149">此过程可能需要多达 24 小时。</span><span class="sxs-lookup"><span data-stu-id="56b87-149">This process might take up to 24 hours.</span></span>
5. <span data-ttu-id="56b87-150">有关还原已删除组的信息，请参阅 在 Azure Active Directory [还原已删除的 Office 365](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)。</span><span class="sxs-lookup"><span data-stu-id="56b87-150">For more information on restoring a deleted group, see [Restore a deleted Office 365 group in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>

<span data-ttu-id="56b87-151">**组过期策略配置**</span><span class="sxs-lookup"><span data-stu-id="56b87-151">**Group expiration policy configuration**</span></span>

1. <span data-ttu-id="56b87-152">仅 Office 365 组支持此功能，不支持安全组和通讯组此功能。</span><span class="sxs-lookup"><span data-stu-id="56b87-152">This functionality is only supported for Office 365 groups, and not for security groups and distribution groups are not supported.</span></span>
2. <span data-ttu-id="56b87-153">为 Office 365 组配置和使用过期策略需要 Azure AD Premium 许可证。</span><span class="sxs-lookup"><span data-stu-id="56b87-153">Configuring and using the expiration policy for Office 365 groups requires an Azure AD Premium license.</span></span>
3. <span data-ttu-id="56b87-154">目前，在租户上只能为 Office 365 组配置一个过期策略。</span><span class="sxs-lookup"><span data-stu-id="56b87-154">Currently, only one expiration policy can be configured for Office 365 groups on a tenant.</span></span>
4. <span data-ttu-id="56b87-155">只有全局管理员、组管理员、用户管理员和组的所有者才能续订组。</span><span class="sxs-lookup"><span data-stu-id="56b87-155">Only Global administrators, group administrators, user administrators, and the owner of the group can be able to renew a group.</span></span>
5. <span data-ttu-id="56b87-156">如果某个 Office 365 组已过期，则它会被删除，且只能在永久删除发生前 30 天内还原。</span><span class="sxs-lookup"><span data-stu-id="56b87-156">If an Office 365 group is expired, it is deleted and can only be restored up to 30 days before permanent deletion occurs.</span></span> <span data-ttu-id="56b87-157">永久删除后，无法再还原组。</span><span class="sxs-lookup"><span data-stu-id="56b87-157">Once permanently deleted, the group can no longer be restored.</span></span> <span data-ttu-id="56b87-158">在[此处](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)了解有关还原组。</span><span class="sxs-lookup"><span data-stu-id="56b87-158">Learn more about restoring groups [here](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>

<span data-ttu-id="56b87-159">**基于活动的自动续订**</span><span class="sxs-lookup"><span data-stu-id="56b87-159">**Activity-based automatic renewal**</span></span>

<span data-ttu-id="56b87-160">SharePoint、Outlook 和 Teams 中的用户活动可触发组自动续订。</span><span class="sxs-lookup"><span data-stu-id="56b87-160">User activities from SharePoint, Outlook and Teams can trigger group automatic renewal.</span></span> <span data-ttu-id="56b87-161">在组过期前 35 天检查活动。</span><span class="sxs-lookup"><span data-stu-id="56b87-161">Activities are checked at 35 days before a group expires.</span></span> <span data-ttu-id="56b87-162">如果当前组生命周期内存在活动，将自动续订组，且不会向组所有者发送电子邮件通知。</span><span class="sxs-lookup"><span data-stu-id="56b87-162">If there is activity during the current group lifecycle, the group will be automatically renewed and email notification won't be sent out to group owners.</span></span>

<span data-ttu-id="56b87-163">**已过期组的通知计时**</span><span class="sxs-lookup"><span data-stu-id="56b87-163">**Notification timing for expired groups**</span></span>

1. <span data-ttu-id="56b87-164">电子邮件通知在组到期前 30 天、15 天和 1 天向 Office 365 组所有者发送。</span><span class="sxs-lookup"><span data-stu-id="56b87-164">Email notifications are sent to the Office 365 group owners 30 days, 15 days, and 1 day prior to expiration of the group.</span></span>
2. <span data-ttu-id="56b87-165">首次设置过期时，超过到期时间间隔的任何组均设置为过期前 35 天。</span><span class="sxs-lookup"><span data-stu-id="56b87-165">When you first set up expiration, any groups that are older than the expiration interval are set to 35 days until expiration.</span></span>
3. <span data-ttu-id="56b87-166">组到期日期基于组的续订日期而不是策略更新日期计算。</span><span class="sxs-lookup"><span data-stu-id="56b87-166">Group expiration date is calculated based on the group’s renewal date, not based on the policy updated date.</span></span> <span data-ttu-id="56b87-167">如果更新了过期策略，到期日期将不会更改。</span><span class="sxs-lookup"><span data-stu-id="56b87-167">If the expiration policy is updated, the expiration date will not change.</span></span>
4. <span data-ttu-id="56b87-168">有关详细信息，请参阅 [Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) 中的和续订电子邮件 [还原已删除的 Office 365](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)。</span><span class="sxs-lookup"><span data-stu-id="56b87-168">For more information see, [Group Expiration policy and renewal emails](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) and [Restore a deleted Office 365 group in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>

<span data-ttu-id="56b87-169">**创建组的权限**</span><span class="sxs-lookup"><span data-stu-id="56b87-169">**Permission to create a group**</span></span>

<span data-ttu-id="56b87-170">确保你有权创建新组。</span><span class="sxs-lookup"><span data-stu-id="56b87-170">Ensure that you are authorized to create a new group.</span></span> <span data-ttu-id="56b87-171">全局管理员可在 Azure 门户或访问面板中禁用组创建。</span><span class="sxs-lookup"><span data-stu-id="56b87-171">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="56b87-172">可能需要管理员来新建组或授予你适当的权限。</span><span class="sxs-lookup"><span data-stu-id="56b87-172">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

1. [<span data-ttu-id="56b87-173">在 Azure 门户中创建新组并添加成员</span><span class="sxs-lookup"><span data-stu-id="56b87-173">Create a new group and add members in Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [<span data-ttu-id="56b87-174">在 Powershell MSOnline 中创建组</span><span class="sxs-lookup"><span data-stu-id="56b87-174">Create groups in Powershell MSOnline</span></span>](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [<span data-ttu-id="56b87-175">在 Powershell 中禁用组创建</span><span class="sxs-lookup"><span data-stu-id="56b87-175">Disable groups creation in Powershell</span></span>](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [<span data-ttu-id="56b87-176">管理可在 Office 365 中创建组的成员</span><span class="sxs-lookup"><span data-stu-id="56b87-176">Manage who can create groups in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [<span data-ttu-id="56b87-177">通过 Powershell 禁用 Office 365 欢迎通知</span><span class="sxs-lookup"><span data-stu-id="56b87-177">Disable Office 365 welcome notification via Powershell</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [<span data-ttu-id="56b87-178">Azure AD 管理角色</span><span class="sxs-lookup"><span data-stu-id="56b87-178">Azure AD administrative roles</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

<span data-ttu-id="56b87-179">**管理组创建权限**</span><span class="sxs-lookup"><span data-stu-id="56b87-179">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="56b87-180">全局管理员可通过设置 **用户可以在 Azure 门户** 或 **中创建的安全组或 Office 365 组来管理在 Azure 门户或访问面板中创建的 Office 365 组创建安全组。用户可在 Azure 门户中的** 设置中、"**所有组">"常规（设置）"** 中创建 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="56b87-180">Global administrators can manage group creation permissions for security or Office 365 groups created in the Azure portal or Access Panel, by setting **Users can create security groups in Azure portals** or **Users can create Office 365 groups in Azure portals** settings in **All groups > General (Settings)**.</span></span>
2. <span data-ttu-id="56b87-181">如果拥有 Azure AD P1 Premium 许可证，还可限制组创建，以选择一组用户。</span><span class="sxs-lookup"><span data-stu-id="56b87-181">You can also restrict group creation to select a group of users if you have an Azure AD P1 Premium license.</span></span>

<span data-ttu-id="56b87-182">**禁用对 Office 365 组的新成员的欢迎通知**</span><span class="sxs-lookup"><span data-stu-id="56b87-182">**Disabling welcome notification for new members of an Office 365 group**</span></span>

<span data-ttu-id="56b87-183">通过向添加到 Office 365 组的用户发送的欢迎通知，可在 Powershell 中将 `UnifiedGroupWelcomeMessageEnabled` 设置为 **False** 禁用。</span><span class="sxs-lookup"><span data-stu-id="56b87-183">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting `UnifiedGroupWelcomeMessageEnabled` to **False** in Powershell.</span></span> <span data-ttu-id="56b87-184">在此处了解有关此设置 [，](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)。</span><span class="sxs-lookup"><span data-stu-id="56b87-184">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).</span></span>













