---
title: 将组分配给 Azure AD 角色
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
- "7898"
- "9003230"
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036230"
---
# <a name="assigning-groups-to-azure-ad-role"></a>将组分配给 Azure AD 角色

要将 Azure AD 中具有授权来源的 Azure AD 组分配给 Azure AD 角色，请执行以下步骤：

1. 创建新组 - 以创建新组：

    a. 使用 **特权角色管理员** 或 **全局管理员** 权限登录到 Azure AD 管理中心。
    b. 选择 **Azure Active Directory > 组 > 所有组 > 新建组**。
    c. 创建组。

2. 在组创建期间或在组创建之后将角色分配给组。

    a. 要在创建组时将角色分配给组，请打开 **可以将 Azure AD 角色分配给组** 切换按钮，并创建组。
    b. 要在组创建后将角色分配给该组，请导航到新创建的组的“**已分配角色**”选项卡，然后将角色分配给该组。  

**管理分配给 Azure AD 角色的组的会员资格**

为防止提升权限，默认情况下，只有特权角色管理员和全局管理员才能修改分配给角色的组的会员资格。 但是，他们可以选择为这样的组分配所有者并委派此任务。

有关将云组分配给 Azure AD 角色的更多详细信息，请参阅[将 AD 角色分配给云组](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)。 有关对分配给云组的角色进行疑难解答的更多详细信息，请参阅[对分配给云组的角色进行疑难解答](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)。





