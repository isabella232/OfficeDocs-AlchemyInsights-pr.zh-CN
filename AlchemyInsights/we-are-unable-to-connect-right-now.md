---
title: 激活问题 - 我们现在无法连接
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744585"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>修复Microsoft 365应用"我们现在无法连接"消息

注意：如果你使用的是较旧版本的 Windows (例如 Windows 7 SP1、Windows Server 2008 R2) ，请使用简单修补程序启用 TLS 1.2 作为默认值。 [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) 有关详细信息，请参阅 [更新以在 Windows 的 WinHTTP 中启用 TLS 1.1 和 TLS 1.2 作为默认安全协议](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)。

如果收到此消息，请尝试执行以下操作：

1. 检查防火墙、防病毒软件和代理设置，确认它们不会阻止 Internet 访问 Microsoft 365应用。 请参阅 [Microsoft URL 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。

2. 转到"**开始**  >  **运行**"，然后键入 **services.msc。** 确保以下服务均在运行：
    - 网络连接设备自动设置
    - 网络列表服务
    - 网络位置感知
    - Windows 事件日志

如果其中一个服务未运行，请尝试启动它。 如果在启动服务时遇到问题，请通过打开具有提升的权限的命令提示符来运行以下命令：

**sfc /scannow**

此命令完成后，重新启动计算机。

有关详细信息，请参阅["抱歉，无法连接到您的帐户。请稍后重试"从 Office 激活Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)错误。