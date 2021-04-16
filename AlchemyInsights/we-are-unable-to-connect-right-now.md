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
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806432"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>修复 Microsoft 365 应用"我们现在无法连接"消息

如果收到此消息，请尝试执行以下操作：

1. 请检查防火墙、防病毒软件和代理设置，确认它们不会阻止 Internet 访问 Microsoft 365 应用。 请参阅 [Microsoft URL 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。

2. 转到"**开始**  >  **运行**"，然后键入 **services.msc。** 确保以下服务均在运行：
    - 网络连接设备自动设置
    - 网络列表服务
    - 网络位置感知
    - Windows 事件日志

如果其中一个服务未运行，请尝试启动它。 如果在启动服务时遇到问题，请通过打开具有提升的权限的命令提示符来运行以下命令：

**sfc /scannow**

此命令完成后，重新启动计算机。

有关详细信息，请参阅 ["抱歉，无法连接到您的帐户。从 Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)激活 Office 时，请稍后重试"错误" 。