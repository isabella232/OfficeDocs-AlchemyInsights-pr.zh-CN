---
title: 在 Outlook 中添加加载项时，多个用户收到“拒绝访问”错误
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2020
ms.locfileid: "45397693"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="284f4-102">在 Outlook 中添加加载项时，多个用户收到“拒绝访问”错误</span><span class="sxs-lookup"><span data-stu-id="284f4-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="284f4-103">可以指定组织中的哪些管理员有权安装和管理适用于 Outlook 的加载项。</span><span class="sxs-lookup"><span data-stu-id="284f4-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="284f4-104">还可以指定组织中的哪些用户有权安装和管理供其自己使用的加载项。</span><span class="sxs-lookup"><span data-stu-id="284f4-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="284f4-105">有关详细信息，请参阅[指定可安装和管理 Outlook 加载项的管理员和用户](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)。</span><span class="sxs-lookup"><span data-stu-id="284f4-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="284f4-106">若要验证是否已成功为用户分配权限，请将 <Role Name> 替换为要验证的角色的名称，然后在 Exchange Online PowerShell 中运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="284f4-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="284f4-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="284f4-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="284f4-108">此示例演示如何验证向谁分配了为组织安装 Office 应用商店提供的加载项所需的权限。</span><span class="sxs-lookup"><span data-stu-id="284f4-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="284f4-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="284f4-109">PowerShell</span></span>

<span data-ttu-id="284f4-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="284f4-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="284f4-111">在结果 Get-ManagementRoleAssignment 中，查看“有效用户”列中的条目。</span><span class="sxs-lookup"><span data-stu-id="284f4-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="284f4-112">有关语法和参数的详细信息，请参阅 [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)。</span><span class="sxs-lookup"><span data-stu-id="284f4-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 