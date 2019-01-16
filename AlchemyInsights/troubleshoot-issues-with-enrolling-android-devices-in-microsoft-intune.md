---
title: 解决问题注册中 Microsoft Intune Android 设备
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 2f4fc434128ebe7323f0b8c08aec3be82112bbda
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28278126"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>解决问题注册中 Microsoft Intune Android 设备

查看下列来解决此问题现在资源。
  
一些常见的问题和解决步骤：
  
 **设备不加密的公司门户中的错误：** 较新版本的 Android，特别开头 7.0 版，需要启动密码以确保您的设备完全进行加密。常见的解决方案是启用启动 pin 或完全加密设备。查看[此文档](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)的详细信息。 
  
 **设备无法检查使用 Intune 服务或 Intune 管理控制台中显示为"不正常":** 某些三星 4.4 和 5.5 设备可能未签入该服务。有 3 于此问题可能的解决方案： 
  
1. 手动打开 Intune 的公司门户应用程序，将自动启动设备同步。
    
2. 更新为 Android 6.0 或更高的设备。
    
3. 从管理 Intune 的公司门户中禁用三星智能管理器。查看[此文档](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)有关的详细信息这些问题和解决方法。 
    
 **用户许可证类型无效**或**用户名称无法识别错误：** ，用户需要分配一个 Intune 或 EMS 许可证。查看这些文档，以将通过许可证分配： Office 管理中心或 Azure 门户。 
  
更多资源以帮助解决您的问题：
  
1. 使用[Intune 疑难解答门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)诊断和解决常见注册失败。查看[此文档](https://docs.microsoft.com/en-us/intune/help-desk-operators)的详细信息。 
    
2. 查看[此文档](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune)的每个阻止注册和解析的常见错误列表。 
    
3. [了解如何注册 Microsoft Intune 中的 Android 设备](https://docs.microsoft.com/en-us/intune/android-enroll)。
    

