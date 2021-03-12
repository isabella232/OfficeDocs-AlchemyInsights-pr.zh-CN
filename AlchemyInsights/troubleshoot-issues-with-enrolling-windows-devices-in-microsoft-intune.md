---
title: 解决在 Microsoft Intune 中注册 Windows 设备的问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708880"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>解决在 Microsoft Intune 中注册 Windows 设备的问题

查看下面列出的资源，以现在解决问题。
  
一些常见的错误消息和解决步骤：
  
 **无法安装该软件，0x80cf4017：** 您的帐户证书已过期。 在 Intune 管理控制台中重新下载电脑客户端软件包。 有关详细信息，请查看本文档。
  
 **错误代码0x801c0003：** 在下列情况下可能发生此错误：
  
-  用户注册的设备数超过设备限制。 查看这些文档[以删除设备或](https://docs.microsoft.com/intune/devices-wipe)[更改设备限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。

-  "用户可以将设备加入 Azure AD"设置为"无"。 将其设置为所有用户或选择用户。 有关详细信息 [，](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) 请查看本文档。

-  设备已由其他用户注册。 如果是这种情况，请从 Azure Intune 控制台中删除设备，或在重试之前手动取消注册设备。

-  设备是 Windows 10 家庭版本。 只有 Windows 10 专业版、教育版和企业版 SKUS 才能加入 Azure Active Directory。

有助于解决问题的其他资源：
  
-  使用 [Intune 故障排除门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 诊断和解决常见的注册失败。 有关详细信息 [，](https://docs.microsoft.com/intune/help-desk-operators) 请查看本文档。

-  有关阻止注册的一系列常见错误及其解决方案，请查看以下文档：[故障排除指南](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)和[疑难解答文档](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)。

[了解如何在 Microsoft Intune 中注册 Windows 设备](https://docs.microsoft.com/intune/windows-enroll)。
