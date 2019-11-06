---
title: 2609-保留-或-电子数据展示-保留
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994046"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="20d1c-102">无法删除 SharePoint Online 或 OneDrive for Business 中的项目</span><span class="sxs-lookup"><span data-stu-id="20d1c-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="20d1c-103">您或您的用户可能无法删除 SharePoint Online 或 OneDrive for Business 中的项目，因为保留策略、保留标签或电子数据展示保留适用于 OneDrive 站点的 SharePoint 或特定项目。</span><span class="sxs-lookup"><span data-stu-id="20d1c-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="20d1c-104">这包括无法删除文档、文档版本、文件夹、文档库、列表、应用程序、网站或网站集。</span><span class="sxs-lookup"><span data-stu-id="20d1c-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="20d1c-105">下面是您在尝试删除要保留的项目时可能收到的错误消息的一些示例：</span><span class="sxs-lookup"><span data-stu-id="20d1c-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="20d1c-106">"此网站包含在电子数据展示保留或保留策略中，无法删除"</span><span class="sxs-lookup"><span data-stu-id="20d1c-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="20d1c-107">"此网站的合规性策略设置为阻止删除"</span><span class="sxs-lookup"><span data-stu-id="20d1c-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="20d1c-108">"合规性策略目前阻止此网站删除"</span><span class="sxs-lookup"><span data-stu-id="20d1c-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="20d1c-109">"无法删除此网站集，因为它包含电子数据展示保留或保留策略中包含的网站"</span><span class="sxs-lookup"><span data-stu-id="20d1c-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="20d1c-110">"在删除文件夹之前，您必须删除此文件夹中的所有项目"</span><span class="sxs-lookup"><span data-stu-id="20d1c-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="20d1c-111">"无法删除此项的版本，因为它处于保留或保留策略中"</span><span class="sxs-lookup"><span data-stu-id="20d1c-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="20d1c-112">"保留时无法删除项目"</span><span class="sxs-lookup"><span data-stu-id="20d1c-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="20d1c-113">"应用于此项的标签阻止对其进行编辑或删除"</span><span class="sxs-lookup"><span data-stu-id="20d1c-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="20d1c-114">"保留策略时无法删除列表" 或 "保留策略"</span><span class="sxs-lookup"><span data-stu-id="20d1c-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="20d1c-115">如果列表被阻止或应用了保留策略，则无法删除该列表</span><span class="sxs-lookup"><span data-stu-id="20d1c-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="20d1c-116">若要删除其中一个方案中的项目，必须删除保留策略、保留标签或电子数据展示保留（或必须从保留策略中排除某个网站）。</span><span class="sxs-lookup"><span data-stu-id="20d1c-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="20d1c-117">您需要禁用或排除导致此问题的相应保留。</span><span class="sxs-lookup"><span data-stu-id="20d1c-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="20d1c-118">在删除保留策略或保留后，可能需要长达24小时才能使更改生效。</span><span class="sxs-lookup"><span data-stu-id="20d1c-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="20d1c-119">有关可应用于 SharePoint 网站和 OneDrive 帐户的不同保留和保留功能的信息，请参阅下列主题之一。</span><span class="sxs-lookup"><span data-stu-id="20d1c-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="20d1c-120">保留策略概述</span><span class="sxs-lookup"><span data-stu-id="20d1c-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="20d1c-121">保留标签概述</span><span class="sxs-lookup"><span data-stu-id="20d1c-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="20d1c-122">在高级电子数据展示中管理保留</span><span class="sxs-lookup"><span data-stu-id="20d1c-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="20d1c-123">电子数据展示保留</span><span class="sxs-lookup"><span data-stu-id="20d1c-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="20d1c-124">旧版网站关闭和删除策略</span><span class="sxs-lookup"><span data-stu-id="20d1c-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
