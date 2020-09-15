---
title: 将驱动器映射到 SharePoint 时访问被拒绝
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 8fc866390d63443c94beef76b6a53a628b85d6d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668733"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="90a72-102">解决映射到网络驱动器的 SharePoint 库的问题</span><span class="sxs-lookup"><span data-stu-id="90a72-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="90a72-103">当您浏览到映射的网络驱动器时，您可能会看到以下消息之一：</span><span class="sxs-lookup"><span data-stu-id="90a72-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="90a72-104">**\\路径不可访问。您可能没有使用此网络资源的权限。若要了解您是否具有访问权限，请与此服务器的管理员联系。**</span><span class="sxs-lookup"><span data-stu-id="90a72-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="90a72-105">**访问被拒绝。在此位置打开文件之前，必须首先将网站添加到受信任的网站列表中，浏览到网站，然后选择 "自动登录" 选项。**</span><span class="sxs-lookup"><span data-stu-id="90a72-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="90a72-106">[获取有关映射的网络驱动器疑难解答的帮助](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)。</span><span class="sxs-lookup"><span data-stu-id="90a72-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="90a72-107">将库映射为网络驱动器是临时性的，并且仅在 Internet Explorer 中受支持。</span><span class="sxs-lookup"><span data-stu-id="90a72-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="90a72-108">相反，请 [使用新的 OneDrive 同步客户端同步 SharePoint 文件](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) ，其中包括 ["按需" 文件](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)。</span><span class="sxs-lookup"><span data-stu-id="90a72-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="90a72-109">无需本地存储空间即可访问所有 OneDrive 中的文件。</span><span class="sxs-lookup"><span data-stu-id="90a72-109">Access all your files in OneDrive without using local storage space.</span></span>
  