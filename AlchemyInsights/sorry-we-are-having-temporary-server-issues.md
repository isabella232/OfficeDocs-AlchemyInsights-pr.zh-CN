---
title: 修复Microsoft 365抱歉，我们收到临时服务器问题消息
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
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021586"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>修复Microsoft 365"抱歉，我们遇到临时服务器问题"消息

如果收到此消息，请尝试执行以下操作：

1. 请检查防火墙、防病毒软件和代理设置，以确认它们不会阻止 Internet 访问 Microsoft 365应用。 请参阅 [URL 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。

2. 转到"**开始**  >  **运行**"，然后键入 **services.msc。** 确保以下服务均在运行：
    - 网络连接设备自动设置
    - 网络列表服务
    - 网络位置感知
    - Windows 事件日志

如果其中一个服务未运行，请尝试启动它。 如果在启动服务时遇到问题，请通过打开具有提升的权限的命令提示符来运行以下命令：

**sfc /scannow**

此命令完成后，重新启动计算机。

有关详细信息，请参阅["抱歉，无法连接到您的帐户。请在激活 时重试"错误"。](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)