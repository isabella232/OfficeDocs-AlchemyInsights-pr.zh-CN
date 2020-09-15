---
title: 访问被拒绝邮件疑难解答
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690773"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="33773-102">访问被拒绝邮件疑难解答</span><span class="sxs-lookup"><span data-stu-id="33773-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="33773-103">如果有人对 SharePoint 中的共享文件夹收到 "拒绝访问" 消息，则网站集管理员可能已启用 "受限访问用户权限锁定模式"。</span><span class="sxs-lookup"><span data-stu-id="33773-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="33773-104">要禁用此功能，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="33773-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="33773-105">浏览到网站，单击 "设置" 图标，然后单击 " **网站设置**"。</span><span class="sxs-lookup"><span data-stu-id="33773-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="33773-106">在“网站集管理”\*\*\*\* 下，单击“网站集功能”\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="33773-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="33773-107">在 " **受限访问用户权限锁定模式**" 旁边，单击 " **停用**"。</span><span class="sxs-lookup"><span data-stu-id="33773-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="33773-108">如果网站是发布网站，则也可能对共享文件夹发生访问被拒绝消息。</span><span class="sxs-lookup"><span data-stu-id="33773-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="33773-109">有关信息，请参阅访问 [共享文件夹时访问被拒绝](https://go.microsoft.com/fwlink/?linkid=2004317)。</span><span class="sxs-lookup"><span data-stu-id="33773-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="33773-110">如果某个人在尝试查看访问请求时收到 "拒绝访问" 消息，则需要将该用户添加为网站集管理员或网站的 "所有者" 组的成员。</span><span class="sxs-lookup"><span data-stu-id="33773-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="33773-111">有关详细信息，请参阅访问 [请求的访问被拒绝列表](https://go.microsoft.com/fwlink/?linkid=2004220)。</span><span class="sxs-lookup"><span data-stu-id="33773-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="33773-112">如果用户从本地 Active Directory 中删除后，如果用户收到 "拒绝访问" 消息，请参阅 [在将用户帐户同步到 Microsoft 365 时，访问被拒绝](https://go.microsoft.com/fwlink/?linkid=2004318)。</span><span class="sxs-lookup"><span data-stu-id="33773-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

