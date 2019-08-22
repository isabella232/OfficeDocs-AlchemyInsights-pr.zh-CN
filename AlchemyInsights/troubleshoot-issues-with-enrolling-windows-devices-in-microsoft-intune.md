---
title: 解决在 Microsoft Intune 中注册 Windows 设备时出现的问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: be66135b80f32f78266ef2b6a7b3f5b30e24d5fc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559618"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>解决在 Microsoft Intune 中注册 Windows 设备时出现的问题

立即查看下面列出的资源, 以解决问题。
  
一些常见的错误消息和解决步骤:
  
 **无法安装软件, 0x80cf4017:** 你的帐户证书已过期。 在 Intune 管理控制台中重新下载 PC 客户端软件程序包。 有关详细信息, 请参阅本文档。
  
 **错误代码 0x801c0003:** 在下列情况下可能会发生此错误:
  
1. 用户已注册的设备超过设备限制。 查看这些文档以[删除设备](https://docs.microsoft.com/intune/devices-wipe)或[更改设备限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。

2. "用户可以将设备加入 Azure AD" 设置为 "无"。 将其设置为 "所有用户" 或 "选择用户"。 有关详细信息, 请参阅[本文档](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)。

3. 设备已由其他用户注册。 如果是这种情况, 请从 Azure Intune 控制台中删除该设备, 或手动取消注册该设备, 然后重试。

4. 设备是 Windows 10 家庭版。 仅 Windows 10 专业版、教育版和企业版 Sku 可以加入 Azure Active Directory。

帮助解决你的问题的其他资源:
  
1. 使用[Intune 故障排除门户](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)诊断和解决常见注册故障。 有关详细信息, 请查看[此文档](https://docs.microsoft.com/intune/help-desk-operators)。

2. 查看这些文档, 了解阻止对每个的注册和解决的常见错误的列表:[故障排除指南](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)和[疑难解答文档](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。

[了解如何在 Microsoft Intune 中注册 Windows 设备](https://docs.microsoft.com/intune/windows-enroll)。
