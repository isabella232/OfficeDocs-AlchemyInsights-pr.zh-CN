---
title: 使用 Intune 查找丢失的 iOS 设备
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434569"
---
# <a name="locating-lost-ios-devices-with-intune"></a>使用 Intune 查找丢失的 iOS 设备

启用 iOS 设备上的丢失模式后，管理员可在锁屏上显示邮件和联系人电话号码。

启用丢失模式后，管理员可以使用“查找设备”操作来识别设备的物理位置。

Intune 中的 "定位设备" 操作适用于 iOS 设备，用于显示特定设备在地图上的位置。

若要执行此操作，iOS 设备必须位于：

- 监督模式
- 丢失模式

有关详细信息，请参阅 [使用 Intune 在 iOS/iPadOS 设备上启用丢失模式](https://docs.microsoft.com/intune/device-lost-mode)，[使用 Intune 找到丢失的或失窃的 iOS/iPadOS 设备](https://docs.microsoft.com/intune/device-locate)。

**常见问题解答**

问：我发出了从设备中删除公司数据的远程操作命令，而现在它处于挂起状态。

答：为了成功完成远程操作，目标设备必须处于联机状态且运行正常。 在以下情况下，远程操作会保持挂起状态 30 天，或除非在以下情形下确认该命令：

- 设备没有连接时
- 设备使用 Intune 失去其管理状态。

如果你认为不会再签入某台设备，并且它不能删除公司数据，请选择“删除”。 删除操作将删除设备记录，使其不再显示在设备的 Intune 列表中。 如果设备再次处于活动状态，则其用户必须重新注册。

问：为什么我无法使用某些远程操作？

答：并非所有平台都支持所有远程设备操作。 以下远程操作是特定于平台的，因此它们仅可用于指定的平台。

- 跳过激活锁（仅限 iOS）
- 全新启动（仅限 Windows）
- 丢失模式（仅限 iOS）
- 定位设备（仅限 iOS）
- 重新启动（仅限 Windows）

有关各项操作的详细信息，请参阅[可用的设备操作](https://docs.microsoft.com/intune/device-management#available-device-actions)。