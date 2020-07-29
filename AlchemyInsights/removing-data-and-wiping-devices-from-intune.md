---
title: 从 Intune 删除数据和擦除设备
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
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434572"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>从 Intune 删除数据和擦除设备

设备停用和设备擦除远程操作可用于删除由 Intune 管理的公司数据或执行出厂重置并将设备恢复为默认设置。

1. 登录 Microsoft 365 设备管理，然后转到“**设备**” > “**所有设备**”。
2. 选择要擦除的设备。
3. 选择要执行的远程擦除类型。 停用只会删除组织信息，而完全擦除会将设备还原为出厂设置。
4. 选择“**是**”进行确认。 在擦除完成之前，设备操作状态将显示为“等待停用”。</br>
    操作完成后，你将不能再在受管理的设备列表中看到该移动设备。

**注意** 无法从已加入 Azure AD 的设备中删除公司数据。

有关停用和擦除操作的影响的完整详细信息（包括保留的内容和删除的内容），请参阅[使用擦除、停用或手动取消注册设备来删除设备](https://docs.microsoft.com/intune/devices-wipe)。

若要擦除 macOS 设备中的所有数据，请参阅[擦除 macOS 设备中的所有数据](https://docs.microsoft.com/intune/device-erase)。