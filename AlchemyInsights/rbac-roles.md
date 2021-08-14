---
title: 'RBAC 角色 '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923118"
---
# <a name="rbac-rules"></a>RBAC 规则

如果收到权限错误： 

- 具有对象 ID 的客户端无权对 (范围代码 **：AuthorizationFailed)** 执行操作：尝试创建资源时，请检查当前是否使用分配了在选定范围内具有资源写入权限的角色的用户登录。 例如，若要管理资源组的虚拟机，应在资源组或父作用域 (虚拟机[](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor)参与者) 。 有关每个内置角色的权限列表，请参阅 Azure 资源的内置 [角色](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)。
- 你无权创建支持请求：当你尝试创建或更新支持票证时，检查你当前是否使用分配了具有 Microsoft.Support/supportTickets/write 权限的角色（如支持请求参与者）的用户登录。 [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- 无法创建其他角色分配 **(代码：RoleAssignmentLimitExceeded)**：尝试分配角色时，请改为尝试通过向组分配角色来减少角色分配的数量。 Azure 支持每个 **订阅最多 2000** 个角色分配。

有关 Azure RBAC 角色的更多详细信息，请参阅 [Azure RBAC 角色](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)。
