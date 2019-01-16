---
title: 解决问题注册 Microsoft Intune 中的 Windows 设备
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28277855"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>解决问题注册 Microsoft Intune 中的 Windows 设备

查看下列来解决此问题现在资源。 
  
某些常见错误消息和解决步骤：
  
 **无法安装该软件，0x80cf4017:** 帐户证书已过期。重新下载 PC 客户端软件程序包 Intune 管理控制台中。查看此文档的详细信息。 
  
 **错误代码 0x801c0003:** 在下列情况下可能会发生错误： 
  
1. 用户具有更多注册超过设备限制的设备。查看这些文档给[删除设备](https://docs.microsoft.com/en-us/intune/devices-wipe)或[更改设备限制](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions)。
    
2. "ヘ ・ 络设备到 Azure AD"设置为"none"。设置为 all，或选择用户。查看[此文档](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings)的详细信息。 
    
3. 已由另一个用户注册设备。如果是这样，从 Azure Intune 控制台删除设备或手动 unenroll 设备，然后重试。
    
4. 设备是主 Windows 10。只有 Windows 10 专业人员、 培训和企业 Sku 可以加入 Azure Active Directory。
    
更多资源以帮助解决您的问题：
  
1. 使用[Intune 疑难解答门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)诊断和解决常见注册失败。查看[此文档](https://docs.microsoft.com/en-us/intune/help-desk-operators)的详细信息。 
    
2. 查看这些文档中的每个阻止注册和解析的常见错误列表：[疑难解答指南](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)和[疑难解答文档](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。
    
[了解如何注册 Microsoft Intune 中的 Windows 设备](https://docs.microsoft.com/en-us/intune/windows-enroll)。
  

