---
title: 解决在 Microsoft Intune 中注册 iOS 设备的问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736148"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>解决在 Microsoft Intune 中注册 iOS 设备的问题

立即查看下面列出的资源，以解决问题。 
  
一些常见的错误消息和解决步骤：
  
- 已**达到设备上限**用户已注册的设备超过设备限制。 查看这些文档以[删除设备](https://docs.microsoft.com/intune/devices-wipe)或[更改设备限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。
    
- **不支持此服务。无注册策略：** 需要配置或续订 Apple 推送通知服务（APNS）。 查看[此文档](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get)以了解如何执行此操作的说明。 
    
- **用户许可证类型无效或无法识别用户名称：** 需要向用户分配 Intune 或 EMS 许可证。 查看这些文档以通过以下步骤分配许可证： [Office 管理中心](https://docs.microsoft.com/intune/licenses-assign)或[Azure 门户](https://docs.microsoft.com/azure/active-directory/license-users-groups)。
    
帮助解决你的问题的其他资源：
  
1. 使用[Intune 故障排除门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)诊断和解决常见注册故障。 有关详细信息，请查看[此文档](https://docs.microsoft.com/intune/help-desk-operators)。 
    
2. 查看这些文档，了解阻止对每个的注册和解决的常见错误的列表：[故障排除指南](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)和[疑难解答文档](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。
    
3. [了解如何在 Microsoft Intune 中注册 iOS 设备](https://docs.microsoft.com/intune/ios-enroll)。
    

