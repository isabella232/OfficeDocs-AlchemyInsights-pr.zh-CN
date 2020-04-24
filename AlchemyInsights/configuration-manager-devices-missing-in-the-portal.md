---
title: 门户中缺少 Configuration Manager 设备
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789599"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="2c516-102">门户中缺少 Configuration Manager 设备</span><span class="sxs-lookup"><span data-stu-id="2c516-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="2c516-103">若要使设备同步正常工作，必须可以从托管服务连接点角色的本地服务器访问[所需的 Internet 终结点](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints)。</span><span class="sxs-lookup"><span data-stu-id="2c516-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="2c516-104">若要解决设备同步问题，请查看位于服务连接点上的 **CMGatewaySyncUploadWorker.log**。</span><span class="sxs-lookup"><span data-stu-id="2c516-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="2c516-105">了解有关 [Microsoft Endpoint Manager 中的租户附加](https://docs.microsoft.com/configmgr/tenant-attach/)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2c516-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
