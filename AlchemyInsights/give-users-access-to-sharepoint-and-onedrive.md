---
title: 授予用户对 SharePoint 和 OneDrive 的访问权限
ms.author: kaarins
author: kaarins
manager: scotv
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 1be9763ce7766c6261f0c1dae78ced6727c7a88d
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36523753"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="41d87-102">授予用户对 SharePoint 和 OneDrive 的访问权限</span><span class="sxs-lookup"><span data-stu-id="41d87-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="41d87-103">如果 OneDrive 或 SharePoint 网站对之前有权访问的多个用户不可用, 则可能存在暂时性的服务问题。</span><span class="sxs-lookup"><span data-stu-id="41d87-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="41d87-104">检查服务运行状况仪表板</span><span class="sxs-lookup"><span data-stu-id="41d87-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="41d87-105">如果您希望组织中的人员能够登录并使用 SharePoint 和 OneDrive, 您需要为他们添加帐户, 并确保他们拥有访问 SharePoint 和 OneDrive 的许可证。</span><span class="sxs-lookup"><span data-stu-id="41d87-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="41d87-106">添加用户的最简单方法是在 Microsoft 365 管理中心。</span><span class="sxs-lookup"><span data-stu-id="41d87-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="41d87-107">转到[Microsoft 365 管理中心中的 "活动用户" 页](https://portal.office.com/adminportal/home#/users), 然后单击 "**添加用户**"。</span><span class="sxs-lookup"><span data-stu-id="41d87-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="41d87-108">填写用户的信息, 并确保 "**产品许可证**" 下已分配 "许可证" 并选择 " **SharePoint Online** "。</span><span class="sxs-lookup"><span data-stu-id="41d87-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="41d87-109">请注意, 如果您在组织中允许外部共享, 则用户可以与组织外部的人员共享 SharePoint 和 OneDrive 内容。</span><span class="sxs-lookup"><span data-stu-id="41d87-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="41d87-110">您无需向这些外部用户授予许可证。</span><span class="sxs-lookup"><span data-stu-id="41d87-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="41d87-111">您也不需要为其添加帐户, 除非将 "共享" 设置为 "仅现有外部用户"。</span><span class="sxs-lookup"><span data-stu-id="41d87-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="41d87-112">在这种情况下, 如果人员不在组织的目录中, 则需要在 Azure AD 管理中心中将其添加为来宾用户。</span><span class="sxs-lookup"><span data-stu-id="41d87-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

