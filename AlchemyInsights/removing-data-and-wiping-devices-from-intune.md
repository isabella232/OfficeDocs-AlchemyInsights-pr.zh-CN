---
title: 从 Intune 删除数据和擦除设备
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: f3614a41c1bc92184d7f8a11bd224310fef6aa0cabc8e1db1288bde01ca1cb5a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922193"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>从 Intune 删除数据和擦除设备

设备停用和设备擦除远程操作可用于删除由 Intune 管理的公司数据或执行出厂重置并将设备恢复为默认设置。

1. 登录 Microsoft 365 设备管理，然后转到“**设备**” > “**所有设备**”。
2. 选择要擦除的设备。
3. 选择要执行的远程擦除类型。 停用只会删除组织信息，而完全擦除会将设备还原为出厂设置。
4. 选择“**是**”进行确认。 擦除完成后，"设备"操作状态将显示为" *停用挂起*。
    操作完成后，你将不能再在受管理的设备列表中看到该移动设备。

> [!NOTE]
> 不能从加入 Azure AD 的设备中删除公司数据。 

有关停用和擦除操作的影响的完整详细信息，包括保留内容及删除内容，请参阅以下文档：

- [通过使用擦除、停用或手动取消上卷设备来删除](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)。
- [如何只从 Intune 托管应用擦除企业数据](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [擦除 macOS 设备应用更新](https://docs.microsoft.com/mem/intune/remote-actions/device-erase)。