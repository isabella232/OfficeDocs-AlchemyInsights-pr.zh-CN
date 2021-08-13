---
title: Intune Win32 应用部署
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: d169dc0dd4e3cd9d94681d7db16ce3051677b708df02d3c9bd461855daabb295
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925875"
---
# <a name="intune-win32-app-deployment"></a>Intune Win32 应用部署

Microsoft Intune 允许 Win32 应用程序（包括但不限于 MSI 和 .EXE ）部署到 Windows 10 设备。 使用的部署机制要求目标设备上存在 Intune 管理扩展 (IME)。 将 powershell 脚本或 win32 应用程序部署定向到用户/设备后，将自动安装 IME。

还必须满足一组先决条件才能部署 Win32 应用，其中包括：

- 支持的平台：Windows 10 版本 1607 或更高版本（企业版、专业版和教育版）。
- 支持的体系结构：x86 和 x64。
- 设备管理：已加入 AAD 和自动注册（包括已加入混合域和自动注册组策略）。
- 应用程序包格式：由 [Microsoft Win32 内容准备工具](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)准备的 .**intunewin** 文件。
- 限制：
    - 最大大小：8GB。
    - 不支持的体系结构：ARMs。

有关这些步骤的相关信息，请查看文档“[在 Microsoft Intune 中添加、分配和监控 Win32 应用](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)”。

有关在 Windows 上对应用程序部署（包括 Win32 应用）进行故障排除的详细信息，请参阅以下文档

- [应用安装问题疑难解答](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Win32 应用疑难解答](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)