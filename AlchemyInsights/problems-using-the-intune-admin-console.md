---
title: 使用 Intune 管理控制台时出现的问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522996"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="ee78f-102">使用 Intune 管理控制台时出现的问题</span><span class="sxs-lookup"><span data-stu-id="ee78f-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="ee78f-103">**导航 Intune 管理门户时出现“访问被拒绝”情况。**</span><span class="sxs-lookup"><span data-stu-id="ee78f-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="ee78f-104">如果你是 Intune 自定义角色的成员，请确保将 Intune 或企业移动性套件 (EMS) 许可证分配给你的帐户。</span><span class="sxs-lookup"><span data-stu-id="ee78f-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="ee78f-105">如果你使用 Configuration Manager 来管理设备，请确认你不属于 Configuration Manager MDM 的 Intune 用户集合。</span><span class="sxs-lookup"><span data-stu-id="ee78f-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="ee78f-106">验证是否已在 Intune 角色边栏选项卡中向你分配了适当的基于角色的管理控制 (RBAC) 权限。</span><span class="sxs-lookup"><span data-stu-id="ee78f-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="ee78f-107">确认所使用的组不是通讯组列表。</span><span class="sxs-lookup"><span data-stu-id="ee78f-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="ee78f-108">Microsoft Azure 门户中的 Intune 仅支持属于 Azure Active Directory 安全组的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="ee78f-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="ee78f-109">在 Microsoft Azure 门户 >“**Intune**” > “**组**”中或者在 Microsoft Azure 门户 >“**Azure Active Directory**”中查看你的组。</span><span class="sxs-lookup"><span data-stu-id="ee78f-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="ee78f-110">**用户对分配的 Intune 角色拥有太多权限**</span><span class="sxs-lookup"><span data-stu-id="ee78f-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="ee78f-111">建议用户转到“**Intune**” > “**Intune 角色**” > “**我的权限**” > “**导出**”以查看已授予的权限。</span><span class="sxs-lookup"><span data-stu-id="ee78f-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="ee78f-112">**我向某个角色添加了范围组，但是该角色中的用户仍可查看其他用户或设备。**</span><span class="sxs-lookup"><span data-stu-id="ee78f-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="ee78f-113">范围组不会筛选用户或设备。</span><span class="sxs-lookup"><span data-stu-id="ee78f-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="ee78f-114">范围组：</span><span class="sxs-lookup"><span data-stu-id="ee78f-114">Scope groups:</span></span>

- <span data-ttu-id="ee78f-115">限制用户可以向谁分配策略或应用程序。</span><span class="sxs-lookup"><span data-stu-id="ee78f-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="ee78f-116">仅允许特定用户在设备上运行远程任务。</span><span class="sxs-lookup"><span data-stu-id="ee78f-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="ee78f-117">有关范围组的详细信息，请参阅 [Microsoft Intune 的基于角色的访问控制 (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)。</span><span class="sxs-lookup"><span data-stu-id="ee78f-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="ee78f-118">**我向某个 Intune 角色添加到了用户，但他们仍对 Intune 管理控制台具有完全访问权限。**</span><span class="sxs-lookup"><span data-stu-id="ee78f-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="ee78f-119">在 Microsoft Azure 门户中导航到“Intune”>“**用户**”，并验证用户是否未分配给 Microsoft Azure 门户中的以下任何角色：</span><span class="sxs-lookup"><span data-stu-id="ee78f-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="ee78f-120">全局管理员</span><span class="sxs-lookup"><span data-stu-id="ee78f-120">Global administrator</span></span>
- <span data-ttu-id="ee78f-121">Intune 服务管理员</span><span class="sxs-lookup"><span data-stu-id="ee78f-121">Intune service administrator</span></span>
- <span data-ttu-id="ee78f-122">SharePoint 管理员</span><span class="sxs-lookup"><span data-stu-id="ee78f-122">SharePoint administrator</span></span>

<span data-ttu-id="ee78f-123">有关详细信息，请参阅 [Microsoft Intune 的基于角色的访问控制 (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)。</span><span class="sxs-lookup"><span data-stu-id="ee78f-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="ee78f-124">**访问问题**</span><span class="sxs-lookup"><span data-stu-id="ee78f-124">**Access Issues**</span></span>

<span data-ttu-id="ee78f-125">有关详细信息，请参阅[无法登录到 Office 365、Azure 或 Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)。</span><span class="sxs-lookup"><span data-stu-id="ee78f-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>