---
title: 解决在设备上Windows设备Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a2abb4d0ef5504c496afefe62a80f3fa21c7ec85536e822e402be33b3617b59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981031"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>解决在设备上Windows设备Microsoft Intune

查看下面列出的资源，以现在解决问题。
  
一些常见的错误消息和解决方法步骤：
  
 **无法安装该软件，0x80cf4017：** 你的帐户证书已过期。 在 Intune 管理控制台中重新下载电脑客户端软件包。 有关详细信息，请查看本文档。
  
 **错误代码0x801c0003：** 此错误可能发生在下列情况下：
  
-  用户注册的设备数超过设备限制。 查看这些文档[以删除设备](https://docs.microsoft.com/intune/devices-wipe)[或更改设备限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。

-  "用户可以将设备加入 Azure AD"设置为"无"。 将其设置为所有用户或选择用户。 有关详细信息 [，](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) 请查看本文档。

-  设备已由另一个用户注册。 如果是这种情况，请从 Azure Intune 控制台中删除设备或手动取消注册设备，然后再重试。

-  设备已Windows 10 家庭版。 只有 Windows 10 专业版、教育Enterprise SK 可以加入Azure Active Directory。

有助于解决问题的其他资源：
  
-  使用 [Intune 疑难解答门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 诊断和解决常见的注册失败。 有关详细信息 [，](https://docs.microsoft.com/intune/help-desk-operators) 请查看本文档。

-  有关阻止注册的一系列常见错误及其解决方案，请查看以下文档：[故障排除指南](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)和[疑难解答文档](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)。

[了解如何在 Microsoft Intune 中注册Windows](https://docs.microsoft.com/intune/windows-enroll)设备。
