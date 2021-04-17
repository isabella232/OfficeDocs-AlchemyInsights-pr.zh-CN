---
title: 门户中缺少 Configuration Manager 设备
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: d57659eb928dd8c4653499e65b6e6cd2f021f521
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817234"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="00bfe-102">门户中缺少 Configuration Manager 设备</span><span class="sxs-lookup"><span data-stu-id="00bfe-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="00bfe-103">若要使设备同步正常工作，必须可以从托管服务连接点角色的本地服务器访问[所需的 Internet 终结点](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints)。</span><span class="sxs-lookup"><span data-stu-id="00bfe-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="00bfe-104">若要解决设备同步问题，请查看位于服务连接点上的 **CMGatewaySyncUploadWorker.log**。</span><span class="sxs-lookup"><span data-stu-id="00bfe-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="00bfe-105">了解有关 [Microsoft Endpoint Manager 中的租户附加](https://docs.microsoft.com/configmgr/tenant-attach/)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="00bfe-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
