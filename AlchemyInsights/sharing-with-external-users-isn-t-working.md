---
title: 与外部用户共享不起作用
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691565"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="8298d-102">解决与外部用户共享 SharePoint 内容的问题</span><span class="sxs-lookup"><span data-stu-id="8298d-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="8298d-103">确保为您的组织打开了外部共享：</span><span class="sxs-lookup"><span data-stu-id="8298d-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="8298d-104">转到 [ &amp; Microsoft 365 管理中心中的 "服务外接程序" 页](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)，然后单击 " **网站**"。</span><span class="sxs-lookup"><span data-stu-id="8298d-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="8298d-105">确保设置为 "打开"。</span><span class="sxs-lookup"><span data-stu-id="8298d-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="8298d-106">如果选择 "仅现有的外部用户"，请确保外部用户在 Microsoft 365 管理中心中列出。</span><span class="sxs-lookup"><span data-stu-id="8298d-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="8298d-107">请确保为网站打开了外部共享。</span><span class="sxs-lookup"><span data-stu-id="8298d-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="8298d-108">对于经典网站集：</span><span class="sxs-lookup"><span data-stu-id="8298d-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="8298d-109">在新的 SharePoint 管理中心中，在左侧窗格中，单击 " **网站**"。</span><span class="sxs-lookup"><span data-stu-id="8298d-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="8298d-110">选择一个或一网站，然后在功能区上，单击 " **共享**"。</span><span class="sxs-lookup"><span data-stu-id="8298d-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="8298d-111">对于属于 Microsoft 365 组或通信网站的团队网站：</span><span class="sxs-lookup"><span data-stu-id="8298d-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="8298d-112">这些新网站类型的共享设置与组织范围的设置相同，除非组织范围设置允许使用不需要登录的链接共享文件。</span><span class="sxs-lookup"><span data-stu-id="8298d-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="8298d-113">在这种情况下，网站允许与登录的新的和现有的外部用户共享。</span><span class="sxs-lookup"><span data-stu-id="8298d-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="8298d-114">若要更改特定网站的设置，请使用新的 SharePoint 管理中心或 PowerShell。</span><span class="sxs-lookup"><span data-stu-id="8298d-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="8298d-115">[了解详细信息](https://go.microsoft.com/fwlink/?linkid=871863)。</span><span class="sxs-lookup"><span data-stu-id="8298d-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="8298d-116">任何网站的外部共享设置的限制可能高于组织范围的设置，但比组织范围设置更许可。</span><span class="sxs-lookup"><span data-stu-id="8298d-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

