---
title: 使用 Intune 跳过受监督的 iOS 设备上的激活锁
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 743b5917c08b0a49a8c5791bdeb59a1672dd0fc7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757290"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>使用 Intune 跳过受监督的 iOS 设备上的激活锁

通过跳过 iOS 设备上的激活锁，当用户在公司设备上启用激活锁并从公司离职后，你可以更轻松地进行恢复。

跳过激活锁的先决条件包括：

- 设备是“受监督的设备”。
- 已使用 Intune 中的 iOS 设备限制策略成功启用激活锁。

此外，跳过激活锁时，应执行以下操作：

- 实际拥有要擦除的设备。
- 在发出擦除命令之前先复制代码。

**注意：** 擦除代码不区分大小写，因此不需要“-”字符。

有关详细信息，请参阅[使用 Intune 跳过受监督的 iOS 设备上的激活锁](https://docs.microsoft.com/intune/device-activation-lock-bypass)。

**常见问题解答**

问：**我发出了从设备中删除公司数据的远程操作命令，而现在它处于挂起状态。**

答：为了成功完成远程操作，目标设备必须处于联机状态且运行正常。 在以下情况下，远程操作会保持挂起状态 30 天，或除非设备在以下情形下确认该命令：

- 没有连接。
- 使用 Intune 失去其管理状态。

如果你认为不会再签入某台设备，并且它不会删除公司数据，请选择“删除”。 删除操作将删除设备记录，使其不再显示在设备的 Intune 列表中。 为了使该设备再次激活，其用户必须重新注册它。

问：**为什么我无法使用某些远程操作？**

答：并非所有平台都支持所有远程设备操作。 以下远程操作特定于平台。

- 跳过激活锁（仅限 iOS）
- 全新启动（仅限 Windows）
- 丢失模式（仅限 iOS）
- 定位设备（仅限 iOS）
- 重新启动（仅限 Windows）

有关各项操作的详细信息，请参阅[可用的设备操作](https://docs.microsoft.com/intune/device-management#available-device-actions)。