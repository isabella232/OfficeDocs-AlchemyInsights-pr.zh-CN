---
title: 2609-保留-或-电子数据展示-保留
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: dee208560e7576597e20aec897f42432d7973727
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727881"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="4970d-102">无法删除 SharePoint Online 或 OneDrive for Business 中的项目</span><span class="sxs-lookup"><span data-stu-id="4970d-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="4970d-103">您或您的用户可能无法删除 SharePoint Online 或 OneDrive for Business 中的项目，因为保留策略、保留标签或电子数据展示保留适用于 OneDrive 站点的 SharePoint 或特定项目。</span><span class="sxs-lookup"><span data-stu-id="4970d-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="4970d-104">这包括无法删除文档、文档版本、文件夹、文档库、列表、应用程序、网站或网站集。</span><span class="sxs-lookup"><span data-stu-id="4970d-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> 

<span data-ttu-id="4970d-105">若要删除其中一个方案中的项目，必须删除保留策略、保留标签或电子数据展示保留 (或者必须从保留策略) 中排除某个网站。</span><span class="sxs-lookup"><span data-stu-id="4970d-105">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="4970d-106">您需要禁用或排除导致此问题的相应保留。</span><span class="sxs-lookup"><span data-stu-id="4970d-106">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="4970d-107">在删除保留策略或保留后，可能需要长达24小时才能使更改生效。</span><span class="sxs-lookup"><span data-stu-id="4970d-107">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="4970d-108">有关可应用于 SharePoint 网站和 OneDrive 帐户的不同保留和保留功能的信息，请参阅下列主题之一。</span><span class="sxs-lookup"><span data-stu-id="4970d-108">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="4970d-109">保留策略概述</span><span class="sxs-lookup"><span data-stu-id="4970d-109">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)
- [<span data-ttu-id="4970d-110">保留标签概述</span><span class="sxs-lookup"><span data-stu-id="4970d-110">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)
- [<span data-ttu-id="4970d-111">在高级电子数据展示中管理保留</span><span class="sxs-lookup"><span data-stu-id="4970d-111">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)
- [<span data-ttu-id="4970d-112">电子数据展示保留</span><span class="sxs-lookup"><span data-stu-id="4970d-112">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)
- [<span data-ttu-id="4970d-113">旧版网站关闭和删除策略</span><span class="sxs-lookup"><span data-stu-id="4970d-113">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)