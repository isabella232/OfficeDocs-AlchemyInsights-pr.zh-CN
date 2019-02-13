---
title: 与外部用户共享不能正常工作
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 20b538846997c021b6e88596a1e8aff401ea935b
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29900854"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="e3548-102">修复与外部用户共享 SharePoint 内容的问题</span><span class="sxs-lookup"><span data-stu-id="e3548-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="e3548-103">请确保您的组织外部共享已打开：</span><span class="sxs-lookup"><span data-stu-id="e3548-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="e3548-104">转到[服务&amp;加载项在 Office 365 管理中心页](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)，并单击**站点**。</span><span class="sxs-lookup"><span data-stu-id="e3548-104">Go to the [Services &amp; add-ins page in the Office 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="e3548-p101">请确保设置已打开到"开"。如果"仅现有的外部用户"处于选中状态，请确保外部用户是否列在 Office 365 管理中心。</span><span class="sxs-lookup"><span data-stu-id="e3548-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Office 365 admin center.</span></span>
    
<span data-ttu-id="e3548-p102">请确保外部共享其开启网站。为经典网站集：</span><span class="sxs-lookup"><span data-stu-id="e3548-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="e3548-109">在经典 SharePoint 管理中心，在左侧窗格中，单击**网站集**。</span><span class="sxs-lookup"><span data-stu-id="e3548-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="e3548-110">选择或多个站点，然后在功能区上单击**共享**。</span><span class="sxs-lookup"><span data-stu-id="e3548-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="e3548-111">对于属于 Office 365 组中，工作组网站或通信网站：</span><span class="sxs-lookup"><span data-stu-id="e3548-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="e3548-p103">这些新的网站类型具有相同共享设置为您的组织范围的设置，除非组织范围的设置允许共享使用的不需要登录链接的文件。在这种情况下，网站允许与新的和现有登录的外部用户共享。若要更改为特定站点的设置，使用新的 SharePoint 管理员中心 （预览） 或 PowerShell。[了解更多](https://go.microsoft.com/fwlink/?linkid=871863)。</span><span class="sxs-lookup"><span data-stu-id="e3548-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="e3548-116">可以比您组织范围的设置，但不是更 permissive 比组织范围内设置更严格的任何网站的外部共享设置。</span><span class="sxs-lookup"><span data-stu-id="e3548-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

