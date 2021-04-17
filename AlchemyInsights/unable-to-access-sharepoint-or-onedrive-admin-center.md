---
title: 无法访问 SharePoint 或 OneDrive 管理中心
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824425"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="6edbc-102">无法访问 SharePoint 或 OneDrive 管理中心</span><span class="sxs-lookup"><span data-stu-id="6edbc-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="6edbc-103">如果你的 SharePoint 或 OneDrive 管理中心网站无法访问或不可用，则可能存在暂时性服务问题，具体表现为用户在访问 SharePoint 网站或 OneDrive 内容时遇到间歇性延迟或导航错误。</span><span class="sxs-lookup"><span data-stu-id="6edbc-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="6edbc-104">请查看[服务运行状况仪表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)，了解你的组织是否受到影响。</span><span class="sxs-lookup"><span data-stu-id="6edbc-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="6edbc-105">需要向全局和 SharePoint 管理员分配 SharePoint 许可证。</span><span class="sxs-lookup"><span data-stu-id="6edbc-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="6edbc-106">刚分配了 SharePoint 许可证或管理员角色的新创建的帐户在访问 SharePoint 时可能会遇到问题，例如“拒绝访问”或“找不到用户”。</span><span class="sxs-lookup"><span data-stu-id="6edbc-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="6edbc-107">请至少留出 24 小时，以便在我们的整个系统中完成同步。</span><span class="sxs-lookup"><span data-stu-id="6edbc-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="6edbc-108">我们理解，24 小时可能看起来很长。</span><span class="sxs-lookup"><span data-stu-id="6edbc-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="6edbc-109">在许多情况下，我们已经在研究解决方案。</span><span class="sxs-lookup"><span data-stu-id="6edbc-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="6edbc-110">如果允许的访问时间段非常小，则 Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) 用户可能会遇到访问被拒的情况，请参阅[对 PIM 帐户的访问被拒绝](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)。</span><span class="sxs-lookup"><span data-stu-id="6edbc-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>