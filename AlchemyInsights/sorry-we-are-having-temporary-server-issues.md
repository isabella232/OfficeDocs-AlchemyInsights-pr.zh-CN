---
title: 修复 Office 应用程序抱歉，我们暂时出现服务器问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627980"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>修复 Office 应用程序 "很抱歉，出现临时服务器问题" 消息

如果您收到此消息，请尝试以下操作：

1. 检查防火墙、防病毒软件和代理设置以确认他们不会阻止对 Office 应用程序的 Internet 访问。 请参阅[Office 365 url 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。

2. 转到 "**开始** > " "**运行**"，然后键入**services.msc**。 确保以下服务全部运行：
    - 网络连接设备自动设置
    - 网络列表服务
    - 网络位置感知
    - Windows 事件日志

如果其中一项服务未在运行，请尝试启动它。 如果您在启动服务时遇到问题，请通过使用提升的权限打开命令提示符来运行以下命令：

**sfc/scannow**

此命令完成后，重新启动计算机。

有关详细信息，请参阅["很抱歉，我们无法连接到你的帐户。在从 Office 365 激活 Office 时，请稍后重试 "错误"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)。