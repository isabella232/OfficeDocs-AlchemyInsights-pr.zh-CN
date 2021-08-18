---
title: 更新与 MCA 关联的售达地址和帐单支付地址 - 推荐步骤
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004166"
- "7325"
ms.openlocfilehash: 5c0f4e7e92081a60be1f6930100ed08ce91ad545
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320020"
---
# <a name="update-sold-to-and-bill-to-address-associated-to-your-mca---recommended-steps"></a>更新与 MCA 关联的售达地址和帐单支付地址 - 推荐步骤

你可以更新与 MCA 客户协议关联的销售对象和帐单 () 。 

**注意**：只有用户管理员才能更改Azure Active Directory用户配置文件信息。 如果未向用户分配用户管理员角色，请与用户管理员联系。 有关更改用户配置文件的信息，请参阅使用"添加或更新用户的配置文件[Azure Active Directory"。](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**售达地址** - 售达地址是负责计费帐户的组织或个人的地址和联系信息。 它显示在为计费帐户生成的所有发票中。

**帐单邮寄** 地址 - 帐单邮寄地址是负责为计费帐户生成的发票的组织或个人的地址和联系信息。 对于 MCA 的计费帐户，每个计费配置文件都有一个帐单邮寄地址，并且显示在为计费配置文件生成的发票中。

**若要更新销售到地址的 MCA 计费帐户**：

1. 使用电子邮件地址登录 Azure 门户，该地址在 MCA 的计费帐户上具有所有者或参与者角色。
1. 搜索 **成本管理**  +  **计费**。
1. Click **Properties**  >  **Update sold-to**.
1. 输入新地址，然后单击"保存 **"。**

某些帐户需要额外验证才能更新其售达地址。 如果你的帐户需要手动审批，将要求你联系 Azure 支持部门。

**若要更新 MCA 计费帐户地址**： 

1. 使用电子邮件地址登录 Azure 门户，该地址在计费帐户或 MCA 的计费配置文件上具有所有者或参与者角色。
1. 搜索 **成本管理**  +  **计费**。
1. 单击 **"计费** 配置文件"并选择一个计费配置文件以更新帐单地址。
1. 单击 **"属性**  >  **""更新地址"。**
1. 输入新地址，然后单击"保存 **"。**

**推荐文档**

[更改 Azure 帐单帐户的联系人信息](https://docs.microsoft.com/azure/cost-management-billing/manage/change-azure-account-profile)   
[更新计费帐户设置](https://docs.microsoft.com/microsoft-store/update-microsoft-store-for-business-account-settings)  
[了解 Azure 中的 Microsoft 客户协议管理角色](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)