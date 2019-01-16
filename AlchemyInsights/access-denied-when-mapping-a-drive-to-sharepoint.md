---
title: 访问被拒绝时将驱动器映射到 SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 2e37c936d1b908729fe870f13ba6c60047c655c3
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28277574"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="c773f-102">修复问题映射到网络驱动器的 SharePoint 库</span><span class="sxs-lookup"><span data-stu-id="c773f-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="c773f-103">浏览到映射的网络驱动器，您可能会看到以下消息之一：</span><span class="sxs-lookup"><span data-stu-id="c773f-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="c773f-104">**\\路径不可访问。您可能没有使用该网络资源的权限。与此服务器的管理员联系，以找出您是否具有访问权限。**</span><span class="sxs-lookup"><span data-stu-id="c773f-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>
    
- <span data-ttu-id="c773f-105">**访问被拒绝。打开文件之前在此位置，必须先添加到受信任的网站列表的网站，浏览到网站，并选择自动登录选项。**</span><span class="sxs-lookup"><span data-stu-id="c773f-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>
    
<span data-ttu-id="c773f-106">[获取帮助疑难解答映射网络驱动器](https://support.office.com/article/ef399c67-4578-4c3a-adbe-0b489084eabe.aspx)。</span><span class="sxs-lookup"><span data-stu-id="c773f-106">[Get help troubleshooting mapped network drives](https://support.office.com/article/ef399c67-4578-4c3a-adbe-0b489084eabe.aspx).</span></span>
  
<span data-ttu-id="c773f-p101">映射网络驱动器库是临时和 Internet Explorer 中仅支持。而是[同步 SharePoint 文件使用新的 OneDrive 同步客户端](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx)包括[文件需求](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)。不使用本地存储空间访问 OneDrive 中的所有文件。</span><span class="sxs-lookup"><span data-stu-id="c773f-p101">Mapping a library as a network drive is temporary and supported only in Internet Explorer. Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx). Access all your files in OneDrive without using local storage space.</span></span>
  

