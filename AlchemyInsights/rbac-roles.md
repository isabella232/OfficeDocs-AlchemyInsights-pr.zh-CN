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
# <a name="rbac-rules"></a><span data-ttu-id="6f829-102">RBAC 规则</span><span class="sxs-lookup"><span data-stu-id="6f829-102">RBAC rules</span></span>

<span data-ttu-id="6f829-103">如果您收到权限错误：</span><span class="sxs-lookup"><span data-stu-id="6f829-103">If you get the permission error:</span></span> 

- <span data-ttu-id="6f829-104">**具有对象 Id 的客户端无权对作用域执行操作 (代码： AuthorizationFailed)**：当您尝试创建资源时，请检查您当前是否已使用分配有对所选范围内的资源的写入权限的用户登录。</span><span class="sxs-lookup"><span data-stu-id="6f829-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="6f829-105">例如，若要管理资源组中的虚拟机，您应具有资源组中的 [虚拟机参与者](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) 角色 (或父作用域) 。</span><span class="sxs-lookup"><span data-stu-id="6f829-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="6f829-106">有关每个内置角色的权限列表，请参阅 [Azure 资源的内置角色](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="6f829-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="6f829-107">**您没有创建支持请求的权限**：当您尝试创建或更新支持票证时，请检查您当前是否已使用分配有 "Microsoft. 支持/supportTickets/写入" 权限的用户登录，如 [支持请求参与者](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)。</span><span class="sxs-lookup"><span data-stu-id="6f829-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="6f829-108">无法 **(代码中创建更多的角色分配： RoleAssignmentLimitExceeded)**：当您尝试分配角色时，请改为通过将角色分配给组来减少角色分配的数量。</span><span class="sxs-lookup"><span data-stu-id="6f829-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="6f829-109">Azure 支持每个订阅最高为 **2000** 个角色分配。</span><span class="sxs-lookup"><span data-stu-id="6f829-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="6f829-110">有关 Azure RBAC 角色的详细信息，请参阅 [AZURE rbac role](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="6f829-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
