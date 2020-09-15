---
title: 解决在 Microsoft Intune 中注册 Windows 设备时出现的问题
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
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658868"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>解决在 Microsoft Intune 中注册 Windows 设备时出现的问题

立即查看下面列出的资源，以解决问题。
  
一些常见的错误消息和解决步骤：
  
 **无法安装软件，0x80cf4017：** 你的帐户证书已过期。 在 Intune 管理控制台中重新下载 PC 客户端软件程序包。 有关详细信息，请参阅本文档。
  
 **错误代码0x801c0003：** 在下列情况下可能会发生此错误：
  
-  用户已注册的设备超过设备限制。 查看这些文档以 [删除设备](https://docs.microsoft.com/intune/devices-wipe) 或 [更改设备限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。

-  "用户可以将设备加入 Azure AD" 设置为 "无"。 将其设置为 "所有用户" 或 "选择用户"。 有关详细信息，请参阅 [本文档](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) 。

-  设备已由其他用户注册。 如果是这种情况，请从 Azure Intune 控制台中删除该设备，或手动取消注册该设备，然后重试。

-  设备是 Windows 10 家庭版。 仅 Windows 10 专业版、教育版和企业版 Sku 可以加入 Azure Active Directory。

帮助解决你的问题的其他资源：
  
-  使用 [Intune 故障排除门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 诊断和解决常见注册故障。 有关详细信息，请查看 [此文档](https://docs.microsoft.com/intune/help-desk-operators) 。

-  有关阻止注册的一系列常见错误及其解决方案，请查看以下文档：[故障排除指南](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)和[疑难解答文档](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。

[了解如何在 Microsoft Intune 中注册 Windows 设备](https://docs.microsoft.com/intune/windows-enroll)。
