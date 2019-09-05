---
title: 将驱动器映射到 SharePoint 时访问被拒绝
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: c41bfd9d25c8aa946a4ec5156be6d2424f4e2133
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737467"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="1aeb3-102">解决映射到网络驱动器的 SharePoint 库的问题</span><span class="sxs-lookup"><span data-stu-id="1aeb3-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="1aeb3-103">当您浏览到映射的网络驱动器时，您可能会看到以下消息之一：</span><span class="sxs-lookup"><span data-stu-id="1aeb3-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="1aeb3-104">**\\路径不可访问。您可能没有使用此网络资源的权限。若要了解您是否具有访问权限，请与此服务器的管理员联系。**</span><span class="sxs-lookup"><span data-stu-id="1aeb3-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="1aeb3-105">**访问被拒绝。在此位置打开文件之前，必须首先将网站添加到受信任的网站列表中，浏览到网站，然后选择 "自动登录" 选项。**</span><span class="sxs-lookup"><span data-stu-id="1aeb3-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="1aeb3-106">[获取有关映射的网络驱动器疑难解答的帮助](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)。</span><span class="sxs-lookup"><span data-stu-id="1aeb3-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="1aeb3-107">将库映射为网络驱动器是临时性的，并且仅在 Internet Explorer 中受支持。</span><span class="sxs-lookup"><span data-stu-id="1aeb3-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="1aeb3-108">相反，请[使用新的 OneDrive 同步客户端同步 SharePoint 文件](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx)，其中包括["按需" 文件](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)。</span><span class="sxs-lookup"><span data-stu-id="1aeb3-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="1aeb3-109">在不使用本地存储空间的情况下访问 OneDrive 中的所有文件。</span><span class="sxs-lookup"><span data-stu-id="1aeb3-109">Access all your files in OneDrive without using local storage space.</span></span>
  