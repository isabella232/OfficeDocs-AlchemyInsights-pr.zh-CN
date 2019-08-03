---
title: Dynamics 365-在 Dynamics 365 统一接口中显示错误的仪表板
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 6edf6fbae0174f3fa4d635c7a99e7daae1243b60
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747009"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="786f6-102">Dynamics 365 统一接口中显示错误的仪表板</span><span class="sxs-lookup"><span data-stu-id="786f6-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="786f6-103">您可能会看到与您所期望的仪表板不同的仪表板的几个原因:</span><span class="sxs-lookup"><span data-stu-id="786f6-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="786f6-104">用户已设置用户默认仪表板</span><span class="sxs-lookup"><span data-stu-id="786f6-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="786f6-105">通常, 如果 "**设置为默认**值" 按钮未显示在仪表板命令栏中, 则可以标识用户默认仪表板。</span><span class="sxs-lookup"><span data-stu-id="786f6-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="786f6-106">用户默认仪表板将覆盖所有其他默认仪表板, 即使用户的默认仪表板不在当前应用中也是如此。</span><span class="sxs-lookup"><span data-stu-id="786f6-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="786f6-107">使用以下解决方法取消设置其默认仪表板。</span><span class="sxs-lookup"><span data-stu-id="786f6-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="786f6-108">创建新的个人仪表板。</span><span class="sxs-lookup"><span data-stu-id="786f6-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="786f6-109">将该新仪表板设置为用户默认的仪表板。</span><span class="sxs-lookup"><span data-stu-id="786f6-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="786f6-110">删除该仪表板。</span><span class="sxs-lookup"><span data-stu-id="786f6-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="786f6-111">在站点地图中设置仪表板</span><span class="sxs-lookup"><span data-stu-id="786f6-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="786f6-112">您可能已通过选择仪表板并在 "自定义系统" 下选择 "设置为默认值" 来设置组织的默认仪表板。</span><span class="sxs-lookup"><span data-stu-id="786f6-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="786f6-113">但是, 如果用户有权访问, 则在站点地图设计器中定义的仪表板将优先于此仪表板。</span><span class="sxs-lookup"><span data-stu-id="786f6-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="786f6-114">若要让用户看到您已设置为组织默认值的仪表板, 您可以执行以下操作之一:</span><span class="sxs-lookup"><span data-stu-id="786f6-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="786f6-115">在站点地图中设置该仪表板</span><span class="sxs-lookup"><span data-stu-id="786f6-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="786f6-116">删除对那些用户的站点地图定义的仪表板的访问权限</span><span class="sxs-lookup"><span data-stu-id="786f6-116">Remove access to the sitemap defined dashboard for those users</span></span>