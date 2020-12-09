---
title: 如何添加和管理管理员-推荐的步骤
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
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599459"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a>如何添加和管理管理员-推荐的步骤

**编辑订阅管理员或协同管理员**

- 帐户管理员可以编辑这两个角色，而订阅管理员只能在 [Azure 门户](https://ms.portal.azure.com/#home)中更改协同管理员。
- [添加或更改 Azure 订阅管理员](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**更新内部 (的订阅管理员或 Co-Administrator) 订阅。**

服务管理员或协同管理员可通过以下步骤为此操作提供自助服务：

1. 登录到 [Azure 门户](https://ms.portal.azure.com/#home) ，然后单击左侧刀片中的 " **成本管理 + 帐单** "。
2. 单击包含订阅的行项。 这将打开订阅的概述。
3. 在 **订阅** 边栏上，单击 " **属性**"。 
4. 单击 " **服务管理员** " 按钮。
5. 输入要将其设置为服务管理员的用户的电子邮件，然后单击 **"确定"**。

**添加/更改/删除共同管理员**

1. 以服务管理员身份登录到 [Azure 门户](https://ms.portal.azure.com/#home) 。
2. 打开 [订阅](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) 并选择订阅。 只能在订阅范围内分配 (共同管理员。 ) 
3. 导航到 **访问控制 (IAM)**  >  **经典管理员**  >  **添加**  >  **添加协同管理员** 若要打开 "**添加** 共同管理员" 窗格 (如果 "添加合作管理员" 选项已禁用，则表示您没有) 的权限。
4. 选择要添加的用户，然后单击 " **添加**"。

**了解更多信息：**
- [添加协同管理员](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [删除协同管理员](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [更改服务管理员](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [查看帐户管理员](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [使用 RBAC 和 Azure 门户管理访问权限](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**使用 Azure Active Directory (AD) 添加/删除用户**

你可以从 Azure Active Directory (Azure AD) 组织中添加新用户或删除现有用户：

1. 若要添加新用户，请以用户管理员的身份登录到 [Azure 门户](https://ms.portal.azure.com/#home) 组织。
2. 选择 " **Azure Active Directory**"，选择 " **用户** "，然后单击 " **新建用户**"。
3. 在 " **用户** " 页上，填写所需的信息。 单击“**创建**”。 将创建用户并将其添加到你的 Azure AD 租户。

**了解详细信息**：

- [添加新用户](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [删除用户](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [使用 Azure Active Directory 添加或更新用户的配置文件信息](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**推荐的文档**

- [什么是基于角色的访问控制 (RBAC) ？](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [了解 Azure 中的不同角色](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Azure Active Directory 中的管理员角色权限](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [教程：使用 RBAC 和 Azure 门户为用户授予访问权限](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [在 Azure 中解决 RBAC](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [使用 Azure 管理组组织你的资源](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [如何通过电子邮件请求 Azure 发票的副本](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [如何在 Azure 中添加、更新或删除信用卡或借记卡](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [管理 (重新激活/取消/切换) 订阅](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



