---
title: Yammer 许可问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657266"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="42733-102">Yammer 许可问题</span><span class="sxs-lookup"><span data-stu-id="42733-102">Yammer licensing issues</span></span>

<span data-ttu-id="42733-103">所有用户都必须拥有许可证才能使用 Yammer Enterprise 服务，但默认情况下，Yammer 不要求用户拥有访问该服务的许可证。</span><span class="sxs-lookup"><span data-stu-id="42733-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="42733-104">当管理员更改设置以阻止没有 Yammer 许可证的 Microsoft 365 用户时，未分配 Yammer Enterprise 许可证的用户将无法访问 Yammer 服务。</span><span class="sxs-lookup"><span data-stu-id="42733-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="42733-105">有关详细信息，请参阅[在 Office 365 中管理 Yammer 用户许可](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="42733-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="42733-106">删除用户的许可证后，Yammer 磁贴将不再显示，并且其他服务可以通过删除许可证来隐藏功能。</span><span class="sxs-lookup"><span data-stu-id="42733-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="42733-107">在其他情况下，仍可显示功能，但需要分配到许可证后才能进行操作。</span><span class="sxs-lookup"><span data-stu-id="42733-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="42733-108">**没有为用户更新许可证**</span><span class="sxs-lookup"><span data-stu-id="42733-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="42733-109">有时，已向用户分配许可证，但其仍无法访问 Yammer。</span><span class="sxs-lookup"><span data-stu-id="42733-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="42733-110">当批量许可证分配正在进行中时，延迟更容易发生。</span><span class="sxs-lookup"><span data-stu-id="42733-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="42733-111">Yammer 用户的更新顺序有可能与 Azure AD 中许可证的更改顺序不同，因为系统是异步运行的。</span><span class="sxs-lookup"><span data-stu-id="42733-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="42733-112">在开启支持案例来报告许可证同步问题前，请先等待 24 小时。</span><span class="sxs-lookup"><span data-stu-id="42733-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="42733-113">**批量许可证分配**</span><span class="sxs-lookup"><span data-stu-id="42733-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="42733-114">许可证可通过管理中心或 PowerShell 脚本进行分配。</span><span class="sxs-lookup"><span data-stu-id="42733-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="42733-115">有关详细信息，请参阅[向用户分配许可证](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)和[使用 Office 365 PowerShell 向用户帐户分配许可证](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)。</span><span class="sxs-lookup"><span data-stu-id="42733-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="42733-116">Microsoft 支持部门不提供有关创建脚本的帮助，但可提供有关 Yammer 许可证分配的文档。</span><span class="sxs-lookup"><span data-stu-id="42733-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="42733-117">有关详细信息，请参阅[使用 Windows PowerShell 管理 Yammer 许可证](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)。</span><span class="sxs-lookup"><span data-stu-id="42733-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>