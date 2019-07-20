---
title: 设备处于等待注册状态
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000657"
- "2508"
ms.openlocfilehash: 46bb390bd89d82bab8099f15f086746800cb4261
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800205"
---
# <a name="devices-are-in-awaiting-enrollment-state"></a><span data-ttu-id="0edf6-102">设备处于 "等待注册" 状态</span><span class="sxs-lookup"><span data-stu-id="0edf6-102">Devices are in "Awaiting Enrollment" state</span></span>

<span data-ttu-id="0edf6-103">桌面分析没有此设备的诊断数据。</span><span class="sxs-lookup"><span data-stu-id="0edf6-103">Desktop Analytics doesn't have diagnostic data for this device.</span></span> 

<span data-ttu-id="0edf6-104">出现此问题的原因可能是您最近向目标集合中添加了设备, 但尚未发送数据。</span><span class="sxs-lookup"><span data-stu-id="0edf6-104">This issue may occur because you recently added the device to the target collection and it hasn't yet sent data.</span></span> <span data-ttu-id="0edf6-105">这也意味着设备未与服务正常通信, 最新的诊断数据超过了28天。</span><span class="sxs-lookup"><span data-stu-id="0edf6-105">It can also mean the device isn't properly communicating with the service, and the latest diagnostic data is more than 28 days old.</span></span>

<span data-ttu-id="0edf6-106">请确保设备可以与服务通信。</span><span class="sxs-lookup"><span data-stu-id="0edf6-106">Make sure the device can communicate with the service.</span></span> <span data-ttu-id="0edf6-107">有关详细信息, 请参阅 [终结点](https://docs.microsoft.com/sccm/desktop-analytics/enable-data-sharing#endpoints)。</span><span class="sxs-lookup"><span data-stu-id="0edf6-107">For more information, see [Endpoints](https://docs.microsoft.com/sccm/desktop-analytics/enable-data-sharing#endpoints).</span></span>

<span data-ttu-id="0edf6-108">有关 awainting 注册状态的详细信息, 请参阅[Monitor Connection Health](https://docs.microsoft.com/sccm/desktop-analytics/monitor-connection-health#awaiting-enrollment)。</span><span class="sxs-lookup"><span data-stu-id="0edf6-108">For more information about the awainting enrollment status, see [Monitor Connection Health](https://docs.microsoft.com/sccm/desktop-analytics/monitor-connection-health#awaiting-enrollment).</span></span>