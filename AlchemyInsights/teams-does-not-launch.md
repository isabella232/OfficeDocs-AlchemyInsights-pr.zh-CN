---
title: Teams 未启动
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100211"
---
# <a name="teams-doesnt-launch"></a>Teams 未启动

如果尝试打开 Microsoft Teams 但它从未启动，请尝试以下操作：

1. 浏览到 **%appdata%\Microsoft\Teams**。
1. 删除文件夹的内容。
1. 重启计算机，然后尝试启动 Teams。

可能需要重新安装 Teams。 重新安装：

1. 使用控制面板卸载 Teams。
1. 浏览到 **%appdata%\Microsoft\Teams\Application Cache**。
1. 删除文件夹的内容。
1. 浏览到 **%appdata%\Microsoft\teams\Cache**。
1. 删除文件夹的内容。
1. 重新启动计算机，然后下载并安装 Teams。

如果要对无法登录的特定用户在租户上运行诊断，请使用关键字 **TeamsUserUnableToSignIn** 启动新的搜索，然后按照提示进行操作。