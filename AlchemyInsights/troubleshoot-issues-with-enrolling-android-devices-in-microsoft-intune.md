---
title: 解决在 Microsoft Intune 中注册 Android 设备时出现的问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500061"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>解决在 Microsoft Intune 中注册 Android 设备时出现的问题

立即查看下面列出的资源, 以解决问题。
  
一些常见的问题和解决步骤:
  
 **公司门户中的设备未加密错误:** 较新版本的 Android (特别是从7.0 开始) 需要启动密码, 以确保您的设备已完全加密。 常见的解决方案是启用启动 pin 或完全加密设备。 有关详细信息, 请查看[此文档](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)。
  
 在**intune 管理控制台中, 设备无法签入 intune 服务或显示为 "不正常":** 某些 Samsung 4.4 和5.5 设备可能无法签入服务。 有3种可能的解决方案可解决此问题:
  
1. 手动打开 Intune 公司门户应用程序, 这将自动启动设备同步。

2. 将设备更新到 Android 6.0 或更高版本。

3. 禁用 Samsung Smart Manager 管理 Intune 公司门户。 有关这些问题和解决方法的详细信息, 请参阅[本文档](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)。

 **用户许可证类型无效**或**无法识别用户名称错误:** 需要为用户分配 Intune 或 EMS 许可证。 查看这些文档以通过以下步骤分配许可证: Office 管理中心或 Azure 门户。
  
帮助解决你的问题的其他资源:
  
1. 使用[Intune 故障排除门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)诊断和解决常见注册故障。 有关详细信息, 请查看[此文档](https://docs.microsoft.com/intune/help-desk-operators)。

2. 查看[此文档](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune), 了解阻止对每个的注册和解决的常见错误的列表。

3. [了解如何在 Microsoft Intune 中注册 Android 设备](https://docs.microsoft.com/intune/android-enroll)。
