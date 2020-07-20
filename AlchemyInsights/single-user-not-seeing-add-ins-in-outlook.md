---
title: 一名用户在 Outlook 中看不到加载项
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2020
ms.locfileid: "45154548"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="8c41d-102">一名用户在 Outlook 中看不到加载项</span><span class="sxs-lookup"><span data-stu-id="8c41d-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="8c41d-103">该用户属于的角色可能没有正确的 AppsForOfficeEnabled 参数。</span><span class="sxs-lookup"><span data-stu-id="8c41d-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="8c41d-104">请运行以下 cmdlet，检查该用户是否已关联适当的角色：</span><span class="sxs-lookup"><span data-stu-id="8c41d-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="8c41d-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span><span class="sxs-lookup"><span data-stu-id="8c41d-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="8c41d-106">有关详细信息，请参阅[指定可安装和管理 Outlook 加载项的管理员和用户](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)。</span><span class="sxs-lookup"><span data-stu-id="8c41d-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
