---
title: 解决在设备中注册 iOS Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 0aaece95effa468af5c906a8bd07e5b00ffa3df37b4e2cb296d64108efec94e9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54047966"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>解决在设备中注册 iOS Microsoft Intune

查看下面列出的资源，以现在解决问题。 
  
一些常见的错误消息和解决方法步骤：
  
- **已达到设备上限** 用户注册的设备数超过设备限制。 查看这些文档[以删除设备](https://docs.microsoft.com/intune/devices-wipe)[或更改设备限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。
    
- **不支持此服务。无注册策略：** 需要 (或续订 APNS) Apple 推送通知服务。 查看 [本文档](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) ，了解如何操作。 
    
- **用户许可证类型无效或用户名无法识别：** 需要为用户分配 Intune 或 EMS 许可证。 查看以下文档以通过以下方式分配许可证[：Office管理中心或](https://docs.microsoft.com/intune/licenses-assign) [Azure 门户。](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
有助于解决问题的其他资源：
  
1. 使用 [Intune 疑难解答门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 诊断和解决常见的注册失败。 有关详细信息 [，](https://docs.microsoft.com/intune/help-desk-operators) 请查看本文档。 
    
2. 有关阻止注册的一系列常见错误及其解决方案，请查看以下文档：[故障排除指南](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)和[疑难解答文档](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)。
    
3. [了解如何在 Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll)注册 iOS 设备。
    

