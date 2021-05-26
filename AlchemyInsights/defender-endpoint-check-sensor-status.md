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
# <a name="defender-endpoint-check-sensor-status"></a>Defender Endpoint 检查传感器状态

**具有传感器问题的设备** 磁贴位于安全操作仪表板上。 此磁贴提供与单个设备提供传感器数据并与 Defender for Endpoint 服务通信功能的有关信息。 它报告需要关注的设备数、帮助识别有问题的设备，并采取措施更正已知问题。

磁贴上的两个状态指示器提供有关未正确向服务报告的设备数量的信息：

- **配置错误** 设备，这些设备可能将部分传感器数据报告给 Defender for Endpoint 服务，并且可能具有需要更正的配置错误。
- **非活动** 设备，这些设备在上一个月中停止向 Defender for Endpoint 服务报告的时间超过 7 天。

单击任意组将引导你进入“设备”列表，并按你的选择进行筛选。 在“设备”列表中，可以按以下状态筛选运行状况状态列表：

- **活动** 设备，这些设备主动向 Defender for Endpoint 服务报告。
- **配置错误** 设备，这些设备可能将部分传感器数据报告给 Defender for Endpoint 服务，但存在需要更正的配置错误。 配置错误的设备可能具有下列问题之一或多个问题组合：

    - 没有传感器数据 - 设备已停止发送传感器数据。 设备可能会触发有限的警报。
    - 受损的通信 - 与设备通信的能力受损。 发送文件进行深度分析、阻止文件、从网络隔离设备以及其他需要与设备通信的操作可能工作不正常。
- **非活动** 设备，这些设备已停止向 Defender for Endpoint 服务报告。

可以使用导出功能下载 CSV 格式的整个列表。

有关详细信息，请参阅 [在 Microsoft Defender for Endpoint 中检查传感器运行状况](/microsoft-365/security/defender-endpoint/check-sensor-status)。

有关导致设备处于非活动状态或配置错误的原因的详细信息，请参阅 [在 Microsoft Defender for Endpoint 中修复运行状况不正常的传感器](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)。
