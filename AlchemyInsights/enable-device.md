---
title: 启用设备
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8278"
ms.openlocfilehash: 9e4b03dcba7a2c98a5d63213ee49f9ba8f91d670
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255151"
---
# <a name="enable-device"></a><span data-ttu-id="5d6fd-102">启用设备</span><span class="sxs-lookup"><span data-stu-id="5d6fd-102">Enable Device</span></span>

<span data-ttu-id="5d6fd-103">**使用 Powershell 命令启用设备**</span><span class="sxs-lookup"><span data-stu-id="5d6fd-103">**To enable the device using Powershell command**</span></span>

<span data-ttu-id="5d6fd-104">运行以下命令：</span><span class="sxs-lookup"><span data-stu-id="5d6fd-104">Run the following commands:</span></span>

- <span data-ttu-id="5d6fd-105">若要获取设备对象， `Get-MsolDevice -Name <Name>`</span><span class="sxs-lookup"><span data-stu-id="5d6fd-105">To get device object: `Get-MsolDevice -Name <Name>`</span></span>
- <span data-ttu-id="5d6fd-106">若要启用设备， `Enable-MsolDevice -DeviceId <DeviceId>`</span><span class="sxs-lookup"><span data-stu-id="5d6fd-106">To enable device: `Enable-MsolDevice -DeviceId <DeviceId>`</span></span>

<span data-ttu-id="5d6fd-107">有关在托管域上配置混合加入的信息，请参阅["配置混合加入"。](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains)</span><span class="sxs-lookup"><span data-stu-id="5d6fd-107">For more information on Configuring Hybrid Join on managed domains, see [Configure Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-managed-domains).</span></span>
