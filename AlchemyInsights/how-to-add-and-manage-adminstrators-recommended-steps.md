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
ms.openlocfilehash: 48a06fde215e007b6b81b32ab751ca8e4bba522d
ms.sourcegitcommit: 46e24d65cffd37b6988447c6738b3315303bbe13
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58339022"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>如何添加和管理管理员 - 建议的步骤

根据您的问题说明，我们找到了一个解决方案。 大多数客户都能够在遵循我们的文档后自行解决问题。

**编辑订阅管理员或共同管理员**

- 帐户管理员可以编辑这两个角色，而订阅管理员只能在 Azure 门户中更改共同 [管理员](https://ms.portal.azure.com/#home)。
- [添加或更改 Azure 订阅管理员](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**更新内部或 AIRS Co-Administrator订阅 (订阅) 订阅**

服务管理员或共同管理员可通过执行以下步骤自行完成此操作：

1. 登录到 Azure 门户 [，然后单击](https://ms.portal.azure.com/#home) 左侧边栏选项卡中的"成本管理 **+** 计费"。
2. 单击订阅的行项。 这将打开订阅概述。
3. 在"订阅 **"边** 栏选项卡上，单击"**属性"。** 
4. 单击" **服务管理"** 按钮。
5. 输入要设置为服务管理员的用户的电子邮件，然后单击"确定 **"。**

**添加/更改/删除共同管理员**

1. 以服务管理员角色登录到 [Azure](https://ms.portal.azure.com/#home) 门户。
2. 打开 [订阅](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) 并选择订阅。  (只能在订阅范围分配共同管理员) 
3. 导航到访问控制 **(IAM)** 经典管理员 添加共同管理员以打开"添加共同管理员"窗格  >    >    >   (如果禁用了"添加共同管理员"选项，则表示您没有) 。
4. 选择要添加的用户，然后单击"添加 **"。**

**了解更多信息：**
- [添加共同管理员](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [删除共同管理员](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [更改服务管理员](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [查看帐户管理员](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [使用 RBAC 和 Azure 门户管理访问权限](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**使用 AD Azure Active Directory (添加/)**

你可以添加新用户或删除 Azure AD 组织Azure Active Directory (现有) 用户：

1. 若要添加新用户，请以组织的用户管理员角色登录到 [Azure](https://ms.portal.azure.com/#home) 门户。
2. 选择 **"Azure Active Directory"，****选择"用户**"，然后单击"**新建用户"。**
3. 在 **"用户** "页上，填写所需信息。 单击“**创建**”。 用户已创建并添加到 Azure AD 租户。

**了解更多信息**：

- [添加新用户](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [删除用户](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [使用自定义设置添加或更新Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**推荐文档**

- [什么是基于角色的访问控制 (RBAC) ？](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [了解 Azure 中的不同角色](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Azure Active Directory 中的管理员角色权限](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [教程：使用 RBAC 和 Azure 门户为用户授予访问权限](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [Azure 中的 RBAC 疑难解答](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [使用 Azure 管理组组织资源](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [如何通过电子邮件请求 Azure 发票副本](https://azure.microsoft.com/blog/azure-email-invoices/)
- [如何添加、更新或删除 Azure 中的信用卡或借记卡](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [管理 (重新激活/取消/切换) 订阅](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



