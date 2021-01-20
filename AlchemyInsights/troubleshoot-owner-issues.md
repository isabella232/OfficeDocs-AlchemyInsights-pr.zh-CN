---
title: 所有者问题疑难解答
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886779"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="41e3a-102">所有者问题疑难解答</span><span class="sxs-lookup"><span data-stu-id="41e3a-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="41e3a-103">若要故障排除所有者相关的问题，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="41e3a-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="41e3a-104">[添加或更改 Azure 订阅管理员](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners)：Azure Active Directory (Azure AD) 组由组所有者所有和管理。</span><span class="sxs-lookup"><span data-stu-id="41e3a-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="41e3a-105">组所有者可以是用户或服务主体，他们有权管理组，包括会员资格。</span><span class="sxs-lookup"><span data-stu-id="41e3a-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="41e3a-106">只有当前的组所有者或管理组的管理员可以分配组所有者。</span><span class="sxs-lookup"><span data-stu-id="41e3a-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="41e3a-107">组所有者不必是组的成员。</span><span class="sxs-lookup"><span data-stu-id="41e3a-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="41e3a-108">[添加或更改 Azure 订阅管理员](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)：此文章介绍了如何为在订阅范围内使用 Azure RBAC 的用户添加或更改管理员角色。</span><span class="sxs-lookup"><span data-stu-id="41e3a-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="41e3a-109">使用 PowerShell 添加组所有者或应用所有者。</span><span class="sxs-lookup"><span data-stu-id="41e3a-109">Use PowerShell to add a group owner or an application owner.</span></span>
