---
title: 性能问题-SharePoint 或 OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719507"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="a779f-102">SharePoint 或 OneDrive 速度慢、对多个用户不可访问或不可用</span><span class="sxs-lookup"><span data-stu-id="a779f-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="a779f-103">如果 OneDrive 或 SharePoint 网站对之前有权访问的多个用户不可用, 则可能存在暂时性的服务问题。</span><span class="sxs-lookup"><span data-stu-id="a779f-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="a779f-104">[检查服务运行状况仪表板](https://portal.office.com/adminportal/home#/servicehealth)。</span><span class="sxs-lookup"><span data-stu-id="a779f-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="a779f-105">添加和许可用户</span><span class="sxs-lookup"><span data-stu-id="a779f-105">Add and license the user</span></span>

<span data-ttu-id="a779f-106">确保[将许可证分配给 Office 365 for business 中的用户](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)。</span><span class="sxs-lookup"><span data-stu-id="a779f-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


## <a name="assign-permissions"></a><span data-ttu-id="a779f-107">分配权限</span><span class="sxs-lookup"><span data-stu-id="a779f-107">Assign Permissions</span></span>

<span data-ttu-id="a779f-108">如果已为用户分配了 Sharepoint 许可证, 但仍收到 "拒绝访问" 消息, 请确保已为其分配了[适当的权限级别](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels)。</span><span class="sxs-lookup"><span data-stu-id="a779f-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) assigned.</span></span>

## <a name="consider-using-the-access-request-feature"></a><span data-ttu-id="a779f-109">考虑使用访问请求功能</span><span class="sxs-lookup"><span data-stu-id="a779f-109">Consider using the access request feature</span></span>

<span data-ttu-id="a779f-110">[访问请求功能](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)允许用户请求对他们当前无权查看的内容的访问权限。</span><span class="sxs-lookup"><span data-stu-id="a779f-110">The [access request feature](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

## <a name="allow-custom-script-may-cause-access-denied-issues"></a><span data-ttu-id="a779f-111">允许自定义脚本可能导致访问被拒绝问题</span><span class="sxs-lookup"><span data-stu-id="a779f-111">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="a779f-112">在某些情况下, 可能会出现 "*允许自定义脚本*" 功能显示访问被拒绝的情况。</span><span class="sxs-lookup"><span data-stu-id="a779f-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="a779f-113">有关受影响的功能的列表、安全注意事项和禁用该功能的功能。</span><span class="sxs-lookup"><span data-stu-id="a779f-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="a779f-114">请访问[允许或阻止自定义脚本](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script)。</span><span class="sxs-lookup"><span data-stu-id="a779f-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>

