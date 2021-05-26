---
title: Defender Endpoint 检查传感器状态
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2021
ms.locfileid: "52627227"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="604a9-102">Defender Endpoint 检查传感器状态</span><span class="sxs-lookup"><span data-stu-id="604a9-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="604a9-103">**具有传感器问题的设备** 磁贴位于安全操作仪表板上。</span><span class="sxs-lookup"><span data-stu-id="604a9-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="604a9-104">此磁贴提供与单个设备提供传感器数据并与 Defender for Endpoint 服务通信功能的有关信息。</span><span class="sxs-lookup"><span data-stu-id="604a9-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="604a9-105">它报告需要关注的设备数、帮助识别有问题的设备，并采取措施更正已知问题。</span><span class="sxs-lookup"><span data-stu-id="604a9-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="604a9-106">磁贴上的两个状态指示器提供有关未正确向服务报告的设备数量的信息：</span><span class="sxs-lookup"><span data-stu-id="604a9-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="604a9-107">**配置错误** 设备，这些设备可能将部分传感器数据报告给 Defender for Endpoint 服务，并且可能具有需要更正的配置错误。</span><span class="sxs-lookup"><span data-stu-id="604a9-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="604a9-108">**非活动** 设备，这些设备在上一个月中停止向 Defender for Endpoint 服务报告的时间超过 7 天。</span><span class="sxs-lookup"><span data-stu-id="604a9-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="604a9-109">单击任意组将引导你进入“设备”列表，并按你的选择进行筛选。</span><span class="sxs-lookup"><span data-stu-id="604a9-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="604a9-110">在“设备”列表中，可以按以下状态筛选运行状况状态列表：</span><span class="sxs-lookup"><span data-stu-id="604a9-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="604a9-111">**活动** 设备，这些设备主动向 Defender for Endpoint 服务报告。</span><span class="sxs-lookup"><span data-stu-id="604a9-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="604a9-112">**配置错误** 设备，这些设备可能将部分传感器数据报告给 Defender for Endpoint 服务，但存在需要更正的配置错误。</span><span class="sxs-lookup"><span data-stu-id="604a9-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="604a9-113">配置错误的设备可能具有下列问题之一或多个问题组合：</span><span class="sxs-lookup"><span data-stu-id="604a9-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="604a9-114">没有传感器数据 - 设备已停止发送传感器数据。</span><span class="sxs-lookup"><span data-stu-id="604a9-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="604a9-115">设备可能会触发有限的警报。</span><span class="sxs-lookup"><span data-stu-id="604a9-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="604a9-116">受损的通信 - 与设备通信的能力受损。</span><span class="sxs-lookup"><span data-stu-id="604a9-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="604a9-117">发送文件进行深度分析、阻止文件、从网络隔离设备以及其他需要与设备通信的操作可能工作不正常。</span><span class="sxs-lookup"><span data-stu-id="604a9-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="604a9-118">**非活动** 设备，这些设备已停止向 Defender for Endpoint 服务报告。</span><span class="sxs-lookup"><span data-stu-id="604a9-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="604a9-119">可以使用导出功能下载 CSV 格式的整个列表。</span><span class="sxs-lookup"><span data-stu-id="604a9-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="604a9-120">有关详细信息，请参阅 [在 Microsoft Defender for Endpoint 中检查传感器运行状况](/microsoft-365/security/defender-endpoint/check-sensor-status)。</span><span class="sxs-lookup"><span data-stu-id="604a9-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="604a9-121">有关导致设备处于非活动状态或配置错误的原因的详细信息，请参阅 [在 Microsoft Defender for Endpoint 中修复运行状况不正常的传感器](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)。</span><span class="sxs-lookup"><span data-stu-id="604a9-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
