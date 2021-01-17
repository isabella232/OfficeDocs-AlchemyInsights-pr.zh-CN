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
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49875344"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="8a38f-102">将组分配给 Azure AD 角色</span><span class="sxs-lookup"><span data-stu-id="8a38f-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="8a38f-103">要将 Azure AD 中具有授权来源的 Azure AD 组分配给 Azure AD 角色，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="8a38f-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="8a38f-104">创建新组 - 以创建新组：</span><span class="sxs-lookup"><span data-stu-id="8a38f-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="8a38f-105">a.</span><span class="sxs-lookup"><span data-stu-id="8a38f-105">a.</span></span> <span data-ttu-id="8a38f-106">使用 **特权角色管理员** 或 **全局管理员** 权限登录到 Azure AD 管理中心。</span><span class="sxs-lookup"><span data-stu-id="8a38f-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="8a38f-107">b.</span><span class="sxs-lookup"><span data-stu-id="8a38f-107">b.</span></span> <span data-ttu-id="8a38f-108">选择 **Azure Active Directory > 组 > 所有组 > 新建组**。</span><span class="sxs-lookup"><span data-stu-id="8a38f-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="8a38f-109">c.</span><span class="sxs-lookup"><span data-stu-id="8a38f-109">c.</span></span> <span data-ttu-id="8a38f-110">创建组。</span><span class="sxs-lookup"><span data-stu-id="8a38f-110">Create the group.</span></span>

2. <span data-ttu-id="8a38f-111">在组创建期间或在组创建之后将角色分配给组。</span><span class="sxs-lookup"><span data-stu-id="8a38f-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="8a38f-112">a.</span><span class="sxs-lookup"><span data-stu-id="8a38f-112">a.</span></span> <span data-ttu-id="8a38f-113">要在创建组时将角色分配给组，请打开 **可以将 Azure AD 角色分配给组** 切换按钮，并创建组。</span><span class="sxs-lookup"><span data-stu-id="8a38f-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="8a38f-114">b.</span><span class="sxs-lookup"><span data-stu-id="8a38f-114">b.</span></span> <span data-ttu-id="8a38f-115">要在组创建后将角色分配给该组，请导航到新创建的组的“**已分配角色**”选项卡，然后将角色分配给该组。</span><span class="sxs-lookup"><span data-stu-id="8a38f-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="8a38f-116">**管理分配给 Azure AD 角色的组的会员资格**</span><span class="sxs-lookup"><span data-stu-id="8a38f-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="8a38f-117">为防止提升权限，默认情况下，只有特权角色管理员和全局管理员才能修改分配给角色的组的会员资格。</span><span class="sxs-lookup"><span data-stu-id="8a38f-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="8a38f-118">但是，他们可以选择为这样的组分配所有者并委派此任务。</span><span class="sxs-lookup"><span data-stu-id="8a38f-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="8a38f-119">有关将云组分配给 Azure AD 角色的更多详细信息，请参阅[将 AD 角色分配给云组](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)。</span><span class="sxs-lookup"><span data-stu-id="8a38f-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="8a38f-120">有关对分配给云组的角色进行疑难解答的更多详细信息，请参阅[对分配给云组的角色进行疑难解答](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)。</span><span class="sxs-lookup"><span data-stu-id="8a38f-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





