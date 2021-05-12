---
title: 从设备清单中删除已载或已停用设备的问题
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2021
ms.locfileid: "52319169"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="51df2-102">从设备清单中删除已载或已停用设备的问题</span><span class="sxs-lookup"><span data-stu-id="51df2-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="51df2-103">Microsoft Defender for Endpoint 当前不允许从设备清单中手动删除载出或停用的设备的设备记录。</span><span class="sxs-lookup"><span data-stu-id="51df2-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="51df2-104">出于安全目的，设备作为历史记录在门户中保留最多 180 天。</span><span class="sxs-lookup"><span data-stu-id="51df2-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="51df2-105">但是，设备数据将按照配置的保留期进行清除。</span><span class="sxs-lookup"><span data-stu-id="51df2-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="51df2-106">**注意：** 载出或停用的设备会在七天后自动 **切换到** 非活动状态。</span><span class="sxs-lookup"><span data-stu-id="51df2-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="51df2-107">此外，过去 30 天内未处于活动状态的设备不会纳入反映组织威胁和漏洞管理曝光分数或 Microsoft 设备安全分数的数据中。</span><span class="sxs-lookup"><span data-stu-id="51df2-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="51df2-108">如果仍不想在"设备清单"视图中看到某些设备，请尝试放置设备标记以从"设备清单"视图中筛选出停用的设备。</span><span class="sxs-lookup"><span data-stu-id="51df2-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="51df2-109">有关详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="51df2-109">For more information, see:</span></span>

[<span data-ttu-id="51df2-110">从 Microsoft Defender for Endpoint 服务载出设备</span><span class="sxs-lookup"><span data-stu-id="51df2-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="51df2-111">威胁和漏洞管理中的曝光评分</span><span class="sxs-lookup"><span data-stu-id="51df2-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="51df2-112">修复 Microsoft Defender for Endpoint 中的不正常传感器</span><span class="sxs-lookup"><span data-stu-id="51df2-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="51df2-113">如何在第 1 部分 (标记) </span><span class="sxs-lookup"><span data-stu-id="51df2-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="51df2-114">如何在第 2 部分 (标记) </span><span class="sxs-lookup"><span data-stu-id="51df2-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="51df2-115">如何在第 3 部分 (标记) </span><span class="sxs-lookup"><span data-stu-id="51df2-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




