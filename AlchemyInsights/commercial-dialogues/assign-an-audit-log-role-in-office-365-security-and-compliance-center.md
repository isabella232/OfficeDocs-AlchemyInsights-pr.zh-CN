---
title: 在 Office 365 安全与合规中心内分配审核日志角色
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735650"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="7c45b-102">在 Office 365 安全与合规中心内分配审核日志角色</span><span class="sxs-lookup"><span data-stu-id="7c45b-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="7c45b-103">若要搜索 Office 365 审核日志，必须在 Exchange Online 中为管理员分配 **仅查看审核日志** 角色或 **审核日志** 角色。</span><span class="sxs-lookup"><span data-stu-id="7c45b-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="7c45b-104">默认情况下，这些角色分配给合规性管理和组织管理角色组。</span><span class="sxs-lookup"><span data-stu-id="7c45b-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="7c45b-105">Office 365 和 Microsoft 365 中的全局管理员将自动添加为组织管理角色组成员。</span><span class="sxs-lookup"><span data-stu-id="7c45b-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="7c45b-106">若要让用户能够使用最低级别权限搜索，可以在 Exchange Online 中创建自定义角色组，添加 **仅供查看审核日志** 或 **审核日志** 角色，然后将用户添加为新角色组的成员。</span><span class="sxs-lookup"><span data-stu-id="7c45b-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="7c45b-107">有关详细信息，请参阅 [在 Exchange Online 中管理角色组](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) 和 [在安全与合规中心中搜索审核日志](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)。</span><span class="sxs-lookup"><span data-stu-id="7c45b-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>