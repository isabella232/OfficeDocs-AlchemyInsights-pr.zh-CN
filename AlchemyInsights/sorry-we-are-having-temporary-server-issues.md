---
title: 正在修复 Microsoft 365 应用程序抱歉，我们暂时出现服务器问题
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758235"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>解决 Microsoft 365 应用程序 "很抱歉，出现临时服务器问题" 消息

如果您收到此消息，请尝试以下操作：

1. 检查你的防火墙、防病毒软件和代理设置以确认他们没有阻止对 Microsoft 365 应用的 Internet 访问。 请参阅 [url 和 IP 地址范围](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)。

2. 转到 "**开始**  >  " "**运行**"，然后键入**services.msc**。 确保以下服务全部运行：
    - 网络连接设备自动设置
    - 网络列表服务
    - 网络位置感知
    - Windows 事件日志

如果其中一项服务未在运行，请尝试启动它。 如果您在启动服务时遇到问题，请通过使用提升的权限打开命令提示符来运行以下命令：

**sfc/scannow**

此命令完成后，重新启动计算机。

有关详细信息，请参阅 ["很抱歉，我们无法连接到你的帐户。请稍后在激活时重试 "错误"](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)。