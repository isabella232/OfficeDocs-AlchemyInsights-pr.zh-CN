---
title: 门户中缺少 Configuration Manager 设备
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4384"
ms.openlocfilehash: b6538cb6a348e194856024680a25af948152910a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812141"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="0da2b-102">门户中缺少 Configuration Manager 设备</span><span class="sxs-lookup"><span data-stu-id="0da2b-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="0da2b-103">若要使设备同步正常工作，必须可以从托管服务连接点角色的本地服务器访问[所需的 Internet 终结点](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints)。</span><span class="sxs-lookup"><span data-stu-id="0da2b-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="0da2b-104">若要解决设备同步问题，请查看位于服务连接点上的 **CMGatewaySyncUploadWorker.log**。</span><span class="sxs-lookup"><span data-stu-id="0da2b-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="0da2b-105">了解有关 [Microsoft Endpoint Manager 中的租户附加](https://docs.microsoft.com/configmgr/tenant-attach/)的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0da2b-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
