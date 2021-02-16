---
title: 组策略
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243894"
---
# <a name="group-policy"></a><span data-ttu-id="342a8-102">组策略</span><span class="sxs-lookup"><span data-stu-id="342a8-102">Group policy</span></span>

<span data-ttu-id="342a8-103">Azure Active Directory 域服务（Azure AD DS）中用户和计算机对象的设置通常使用组策略对象（GPO）进行管理。</span><span class="sxs-lookup"><span data-stu-id="342a8-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="342a8-104">Azure Active Directory 域服务包含AADDC用户和AADDC计算机容器的内置GPO。</span><span class="sxs-lookup"><span data-stu-id="342a8-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="342a8-105">可以自定义这些内置的GPO，根据环境需要配置组策略。</span><span class="sxs-lookup"><span data-stu-id="342a8-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="342a8-106">Azure AD DC 管理员组的成员在 Azure AD DS 域中拥有组策略管理权限，还可以创建自定义 GPO 和组织单位（OU）。</span><span class="sxs-lookup"><span data-stu-id="342a8-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="342a8-107">有关什么是组策略及其工作方式的更多信息，请参阅[组策略概述](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))。</span><span class="sxs-lookup"><span data-stu-id="342a8-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="342a8-108">在混合环境中，在本地 AD DS 环境中配置的组策略不会同步到 Azure AD DS。</span><span class="sxs-lookup"><span data-stu-id="342a8-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="342a8-109">如果要为 Azure AD DS 中的用户或计算机定义配置设置，请编辑其中一个默认 GPO 或创建自定义 GPO。</span><span class="sxs-lookup"><span data-stu-id="342a8-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="342a8-110">本文 [管理组策略](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) 展示了如何安装组策略管理工具，如何编辑内置的GPO，以及如何创建自定义GPO。</span><span class="sxs-lookup"><span data-stu-id="342a8-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



