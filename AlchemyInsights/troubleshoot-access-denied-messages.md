---
title: 访问被拒绝邮件疑难解答
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3973f5bf584343d3353e7389f22bc727827b5c35
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28277606"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="1033e-102">访问被拒绝邮件疑难解答</span><span class="sxs-lookup"><span data-stu-id="1033e-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="1033e-p101">如果某人共享文件夹的"访问被拒绝"消息，网站集管理员可能已经启用了"受限访问用户权限锁定模式。"若要禁用此选项：</span><span class="sxs-lookup"><span data-stu-id="1033e-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="1033e-105">浏览到的网站，单击设置图标，然后单击**网站设置**。</span><span class="sxs-lookup"><span data-stu-id="1033e-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="1033e-106">在**网站集管理**下单击**网站集功能**。</span><span class="sxs-lookup"><span data-stu-id="1033e-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="1033e-107">旁边**有限访问用户权限锁定模式下**，单击**停用**。</span><span class="sxs-lookup"><span data-stu-id="1033e-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="1033e-p102">如果网站是发布网站时，访问被拒绝消息也会发生的共享文件夹。有关信息，请参阅[访问被拒绝访问的共享的文件夹时](https://go.microsoft.com/fwlink/?linkid=2004317)。</span><span class="sxs-lookup"><span data-stu-id="1033e-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="1033e-p103">如果某人得到的"访问被拒绝"消息，尝试查看访问请求时，用户需要被添加为网站集管理员或网站的 Owners 组的成员。有关详细信息，请参阅[访问被拒绝访问请求列表](https://go.microsoft.com/fwlink/?linkid=2004220)。</span><span class="sxs-lookup"><span data-stu-id="1033e-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="1033e-112">如果后从 Active Directory 部署中删除，然后重新添加用户的"访问被拒绝"消息，请参阅[的用户帐户同步到 Office 365 时拒绝访问](https://go.microsoft.com/fwlink/?linkid=2004318)。</span><span class="sxs-lookup"><span data-stu-id="1033e-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

