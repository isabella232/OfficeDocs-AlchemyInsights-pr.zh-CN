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
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576380"
---
# <a name="rbac-rules"></a>RBAC 规则

如果您收到权限错误： 

- **具有对象 Id 的客户端无权对作用域执行操作 (代码： AuthorizationFailed)**：当您尝试创建资源时，请检查您当前是否已使用分配有对所选范围内的资源的写入权限的用户登录。 例如，若要管理资源组中的虚拟机，您应具有资源组中的 [虚拟机参与者](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) 角色 (或父作用域) 。 有关每个内置角色的权限列表，请参阅 [Azure 资源的内置角色](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)。
- **您没有创建支持请求的权限**：当您尝试创建或更新支持票证时，请检查您当前是否已使用分配有 "Microsoft. 支持/supportTickets/写入" 权限的用户登录，如 [支持请求参与者](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)。
- 无法 **(代码中创建更多的角色分配： RoleAssignmentLimitExceeded)**：当您尝试分配角色时，请改为通过将角色分配给组来减少角色分配的数量。 Azure 支持每个订阅最高为 **2000** 个角色分配。

有关 Azure RBAC 角色的详细信息，请参阅 [AZURE rbac role](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)。
