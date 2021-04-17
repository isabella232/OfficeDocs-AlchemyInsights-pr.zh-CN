---
title: 电池无法充电
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
- "9002952"
- "5654"
ms.openlocfilehash: fab76114044f71d60dbaf812cd2cd0cc75c8169c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820456"
---
# <a name="battery-wont-charge"></a>电池无法充电

首先，确保连接安全。 强烈建议仅使用 Microsoft 正版或 Microsoft 许可的电源。

其次，尝试关闭 Surface 并至少充电 30 分钟。 然后将其重新打开以查看问题是否已修复。

**已接通电源，但未充电**

如果任务栏上的电池图标显示“**已接通电源，但未充电**”，则意味着 Surface 检测到电源，但没有对电池充电。 拔出电源后，Surface 可能会关闭。 请尝试使用以下命令：

1. 为 Surface 接通电源。
2. 选择任务栏中的搜索框，键入 **设备管理器**，然后从结果列表中选择“**设备管理器**”。
3. 单击“**电池**”类别旁边的箭头。
4. 双击“**Microsoft Surface ACPI 兼容的控制方法电池**”，选择“**驱动程序**”选项卡，然后单击“**卸载 > 确定**”。
5. 选择“所有类别”顶部的计算机和“**操作**”菜单，然后单击“**扫描硬件更改**”。
6. 使 Surface 保持接电状态。

删除电池驱动程序后，安装 Surface 和 Windows 更新。 有关详细信息，请参阅[更新 Surface 固件和 Windows 10](https://support.microsoft.com/help/4023505)。 检查电池。 如果仍然有问题，请参阅[强制关机并重新启动 Surface](https://support.microsoft.com/help/4036280/surface-force-a-shut-down-and-restart-your-surface)。

**更多疑难解答信息**

电源连接器插入 Surface 时，LED 指示灯应亮起。 如果其状态为关闭、闪烁或闪烁白光，请查看[如果 Surface 电源或充电器无法正常工作，该怎么办](https://support.microsoft.com/help/4484763/surface-fix-issues-with-your-power-supply)。 

如果你的 Surface Book 有问题，请确保屏幕已完全连接到键盘。 如果仍无法充电，请拆下屏幕并使用铅笔橡皮擦清洁连接线。 你可能还需要清洁插入到 Surface 的细长部件上的针脚，并确保将针脚晾干。

若要查看解决电池问题的更多方法，请参阅 [Surface 电池无法充电，或 Surface 无法使用电池](https://support.microsoft.com/help/4023536/surface-surface-battery-wont-charge)。
