---
title: 创建 SharePoint 网站
ms.author: efrene
author: efrene
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 30c51d84005534cc1de9e8b8136da1a07be57b73
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36738187"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="8f7da-102">创建 SharePoint 网站</span><span class="sxs-lookup"><span data-stu-id="8f7da-102">Create a SharePoint site</span></span>

<span data-ttu-id="8f7da-103">您可以参阅以下内容，了解有关 SharePoint 网站创建的信息：</span><span class="sxs-lookup"><span data-stu-id="8f7da-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="8f7da-104">[在新 SharePoint 管理中心中管理网站](https://docs.microsoft.com/sharepoint/manage-site-creation)：了解网站创建选项，包括如何创建经典网站或不包含 Office 365 组的团队网站。</span><span class="sxs-lookup"><span data-stu-id="8f7da-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="8f7da-105">[在 SharePoint 中创建团队网站](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)：了解如何创建团队网站。</span><span class="sxs-lookup"><span data-stu-id="8f7da-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="8f7da-106">[在 SharePoint Online 中创建通信网站](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb)：了解如何创建通信网站。</span><span class="sxs-lookup"><span data-stu-id="8f7da-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="8f7da-107">[在新 SharePoint 管理中心中管理网站](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site)：了解如何创建不包含 Office 365 组的经典网站或团队网站。</span><span class="sxs-lookup"><span data-stu-id="8f7da-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> <span data-ttu-id="8f7da-108">[!几点</span><span class="sxs-lookup"><span data-stu-id="8f7da-108">[!Tips]</span></span>
> - <span data-ttu-id="8f7da-109">您无法使用与现有网站相同的 URL 创建网站。</span><span class="sxs-lookup"><span data-stu-id="8f7da-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="8f7da-110">如果您删除了某个网站，并且希望重新使用该 URL，则可能是已删除的网站仍存在于 "**已删除的网站**" 下。</span><span class="sxs-lookup"><span data-stu-id="8f7da-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="8f7da-111">若要管理已删除的网站，请参阅[删除网站](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)。</span><span class="sxs-lookup"><span data-stu-id="8f7da-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="8f7da-112">若要使用 Powershell 完全删除站点，请参阅[remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet 示例。</span><span class="sxs-lookup"><span data-stu-id="8f7da-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="8f7da-113">某些用户可能不能创建网站。</span><span class="sxs-lookup"><span data-stu-id="8f7da-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="8f7da-114">请参阅[在 SharePoint Online 中管理网站创建](https://docs.microsoft.com/sharepoint/manage-site-creation)。</span><span class="sxs-lookup"><span data-stu-id="8f7da-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="8f7da-115">在**创建**比预期更长的时间，网站可能会变得被卡住。</span><span class="sxs-lookup"><span data-stu-id="8f7da-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="8f7da-116">如果在你首次看到此问题后过去已经超过24小时，请记录一个支持票证。</span><span class="sxs-lookup"><span data-stu-id="8f7da-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="8f7da-117">在许多情况下，我们已经在努力解决了解决方案。</span><span class="sxs-lookup"><span data-stu-id="8f7da-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="8f7da-118">请至少为我们提供24小时的时间来完成解决方案。</span><span class="sxs-lookup"><span data-stu-id="8f7da-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="8f7da-119">如果您需要创建一个不包含 Office 365 组的新团队网站，</span><span class="sxs-lookup"><span data-stu-id="8f7da-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


