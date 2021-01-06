---
title: 如何添加和管理管理员 - 建议的步骤
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755825"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a><span data-ttu-id="f41c9-102">如何添加和管理管理员 - 建议的步骤</span><span class="sxs-lookup"><span data-stu-id="f41c9-102">How to add and manage administrators - recommended steps</span></span>

<span data-ttu-id="f41c9-103">根据您的问题描述，我们提供了一个解决方案。</span><span class="sxs-lookup"><span data-stu-id="f41c9-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="f41c9-104">大多数客户在遵循我们的文档后能够自行解决问题。</span><span class="sxs-lookup"><span data-stu-id="f41c9-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="f41c9-105">**编辑订阅管理员或共同管理员**</span><span class="sxs-lookup"><span data-stu-id="f41c9-105">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="f41c9-106">帐户管理员可以编辑这两个角色，而订阅管理员只能在 Azure 门户中更改共同 [管理员](https://ms.portal.azure.com/#home)。</span><span class="sxs-lookup"><span data-stu-id="f41c9-106">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="f41c9-107">添加或更改 Azure 订阅管理员</span><span class="sxs-lookup"><span data-stu-id="f41c9-107">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="f41c9-108">**更新内部服务 AIRS Co-Administrator 订阅 (订阅) 订阅**</span><span class="sxs-lookup"><span data-stu-id="f41c9-108">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="f41c9-109">服务管理员或共同管理员可通过执行以下步骤自行完成此操作：</span><span class="sxs-lookup"><span data-stu-id="f41c9-109">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="f41c9-110">登录到 Azure [门户，](https://ms.portal.azure.com/#home) 然后单击左侧边栏选项卡中的"成本管理 **+** 计费"。</span><span class="sxs-lookup"><span data-stu-id="f41c9-110">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="f41c9-111">单击订阅的行项。</span><span class="sxs-lookup"><span data-stu-id="f41c9-111">Click on the line item with your subscription.</span></span> <span data-ttu-id="f41c9-112">这将打开订阅的概述。</span><span class="sxs-lookup"><span data-stu-id="f41c9-112">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="f41c9-113">在"**订阅"** 边栏选项卡上，单击"**属性"。**</span><span class="sxs-lookup"><span data-stu-id="f41c9-113">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="f41c9-114">单击 **"服务管理"** 按钮。</span><span class="sxs-lookup"><span data-stu-id="f41c9-114">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="f41c9-115">输入要设置为服务管理员的用户的电子邮件，然后单击"**确定"。**</span><span class="sxs-lookup"><span data-stu-id="f41c9-115">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="f41c9-116">**添加/更改/删除共同管理员**</span><span class="sxs-lookup"><span data-stu-id="f41c9-116">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="f41c9-117">以服务管理员角色登录到 [Azure](https://ms.portal.azure.com/#home) 门户。</span><span class="sxs-lookup"><span data-stu-id="f41c9-117">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="f41c9-118">打开 [订阅](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) 并选择订阅。</span><span class="sxs-lookup"><span data-stu-id="f41c9-118">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="f41c9-119"> (只能在订阅范围分配共同管理员。) </span><span class="sxs-lookup"><span data-stu-id="f41c9-119">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="f41c9-120">导航到访问控制 **(IAM)** 经典管理员添加共同管理员以打开"添加共同管理员"窗格  >    >    >   (如果禁用了"添加共同管理员"选项，则表示您没有权限) 。</span><span class="sxs-lookup"><span data-stu-id="f41c9-120">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="f41c9-121">选择要添加的用户，然后单击"添加 **"。**</span><span class="sxs-lookup"><span data-stu-id="f41c9-121">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="f41c9-122">**了解更多信息：**</span><span class="sxs-lookup"><span data-stu-id="f41c9-122">**Learn more:**</span></span>
- [<span data-ttu-id="f41c9-123">添加共同管理员</span><span class="sxs-lookup"><span data-stu-id="f41c9-123">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="f41c9-124">删除共同管理员</span><span class="sxs-lookup"><span data-stu-id="f41c9-124">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="f41c9-125">更改服务管理员</span><span class="sxs-lookup"><span data-stu-id="f41c9-125">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="f41c9-126">查看帐户管理员</span><span class="sxs-lookup"><span data-stu-id="f41c9-126">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="f41c9-127">使用 RBAC 和 Azure 门户管理访问</span><span class="sxs-lookup"><span data-stu-id="f41c9-127">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="f41c9-128">**使用 Azure Active Directory 和 AD (添加/)**</span><span class="sxs-lookup"><span data-stu-id="f41c9-128">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="f41c9-129">可以在 Azure AD 组织中添加新用户或删除 Azure Active Directory (现有) 用户：</span><span class="sxs-lookup"><span data-stu-id="f41c9-129">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="f41c9-130">若要添加新用户，请以组织的用户管理员角色登录到 [Azure](https://ms.portal.azure.com/#home) 门户。</span><span class="sxs-lookup"><span data-stu-id="f41c9-130">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="f41c9-131">选择 **Azure Active Directory，** 选择 **"用户**"，然后单击 **"新建用户"。**</span><span class="sxs-lookup"><span data-stu-id="f41c9-131">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="f41c9-132">在 **"用户** "页上，填写所需信息。</span><span class="sxs-lookup"><span data-stu-id="f41c9-132">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="f41c9-133">单击“**创建**”。</span><span class="sxs-lookup"><span data-stu-id="f41c9-133">Click **Create**.</span></span> <span data-ttu-id="f41c9-134">用户已创建并添加到 Azure AD 租户。</span><span class="sxs-lookup"><span data-stu-id="f41c9-134">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="f41c9-135">**了解更多信息**：</span><span class="sxs-lookup"><span data-stu-id="f41c9-135">**Learn more**:</span></span>

- [<span data-ttu-id="f41c9-136">添加新用户</span><span class="sxs-lookup"><span data-stu-id="f41c9-136">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="f41c9-137">删除用户</span><span class="sxs-lookup"><span data-stu-id="f41c9-137">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="f41c9-138">使用 Azure Active Directory 添加或更新用户配置文件信息</span><span class="sxs-lookup"><span data-stu-id="f41c9-138">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="f41c9-139">**建议的文档**</span><span class="sxs-lookup"><span data-stu-id="f41c9-139">**Recommended documents**</span></span>

- [<span data-ttu-id="f41c9-140">什么是基于角色的访问控制 (RBAC) ？</span><span class="sxs-lookup"><span data-stu-id="f41c9-140">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="f41c9-141">了解 Azure 中的不同角色</span><span class="sxs-lookup"><span data-stu-id="f41c9-141">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="f41c9-142">Azure Active Directory 中的管理员角色权限</span><span class="sxs-lookup"><span data-stu-id="f41c9-142">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="f41c9-143">教程：使用 RBAC 和 Azure 门户为用户授予访问权限</span><span class="sxs-lookup"><span data-stu-id="f41c9-143">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="f41c9-144">Azure 中的 RBAC 疑难解答</span><span class="sxs-lookup"><span data-stu-id="f41c9-144">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="f41c9-145">使用 Azure 管理组组织资源</span><span class="sxs-lookup"><span data-stu-id="f41c9-145">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="f41c9-146">如何通过电子邮件请求 Azure 发票副本</span><span class="sxs-lookup"><span data-stu-id="f41c9-146">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="f41c9-147">如何添加、更新或删除 Azure 中的信用卡或借记卡</span><span class="sxs-lookup"><span data-stu-id="f41c9-147">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="f41c9-148">管理 (重新激活/取消/切换) 订阅</span><span class="sxs-lookup"><span data-stu-id="f41c9-148">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



