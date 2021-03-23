---
title: 关于 Yammer 管理员
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: fd8534d44c44f2ea8e6b0de8c361109915566868
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2021
ms.locfileid: "50995236"
---
# <a name="about-yammer-admins"></a><span data-ttu-id="50a39-102">关于 Yammer 管理员</span><span class="sxs-lookup"><span data-stu-id="50a39-102">About Yammer admins</span></span>

<span data-ttu-id="50a39-103">**网络管理员**</span><span class="sxs-lookup"><span data-stu-id="50a39-103">**Network admins**</span></span>

<span data-ttu-id="50a39-104">全局管理员将自动提升为 Yammer 网络中已验证的管理员角色。</span><span class="sxs-lookup"><span data-stu-id="50a39-104">Global admins are automatically promoted to the Verified Admin role in a Yammer network.</span></span> <span data-ttu-id="50a39-105">在下列情况下，此升级可能不会正确发生：</span><span class="sxs-lookup"><span data-stu-id="50a39-105">In the following cases, this promotion may not occur correctly:</span></span>

- <span data-ttu-id="50a39-106">存在多个 Yammer 网络，管理员登录的网络错误。</span><span class="sxs-lookup"><span data-stu-id="50a39-106">Multiple Yammer networks exist, and the admin is being signed into the wrong one.</span></span> <span data-ttu-id="50a39-107">[需要网络](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) 整合才能访问一个 Yammer 网络。</span><span class="sxs-lookup"><span data-stu-id="50a39-107">[Network consolidation](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) is required to get to one Yammer network.</span></span>
- <span data-ttu-id="50a39-108">Azure PIM 正在使用中。</span><span class="sxs-lookup"><span data-stu-id="50a39-108">Azure PIM is being used.</span></span> <span data-ttu-id="50a39-109">用户可能不会被提升为全局管理员，因此无法进行推广。</span><span class="sxs-lookup"><span data-stu-id="50a39-109">The user may not be promoted to global admin long enough for the promotion to occur.</span></span> <span data-ttu-id="50a39-110">Yammer 的未来更新可能会解决此问题，但最好是手动将用户提升为全局管理员。</span><span class="sxs-lookup"><span data-stu-id="50a39-110">A future update to Yammer may resolve this issue, but it is best to promote users to global admin manually.</span></span>
- <span data-ttu-id="50a39-111">Yammer 网络存在同步问题。</span><span class="sxs-lookup"><span data-stu-id="50a39-111">A sync issue exists with the Yammer network.</span></span> <span data-ttu-id="50a39-112">在这种情况下，需要进一步调查需要支持请求。</span><span class="sxs-lookup"><span data-stu-id="50a39-112">In this case a support request will be required for further investigation.</span></span>

<span data-ttu-id="50a39-113">有关 Yammer 管理员角色的信息，请参阅 [管理 Yammer 管理员](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)。</span><span class="sxs-lookup"><span data-stu-id="50a39-113">For more information about Yammer admin roles, see [Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins).</span></span>

<span data-ttu-id="50a39-114">**组管理员**</span><span class="sxs-lookup"><span data-stu-id="50a39-114">**Group admins**</span></span>

<span data-ttu-id="50a39-115">Microsoft 365 连接的组的组管理员与 Azure AD 中的组成员身份同步。</span><span class="sxs-lookup"><span data-stu-id="50a39-115">Group admins for Microsoft 365 connected groups are synced with group membership from Azure AD.</span></span> <span data-ttu-id="50a39-116">对于大型组，此同步可能需要一段延长的时间。</span><span class="sxs-lookup"><span data-stu-id="50a39-116">For large groups, this sync can take an extended period.</span></span>
