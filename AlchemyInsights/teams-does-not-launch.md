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
ms.openlocfilehash: ebfabf667092850e5045c56e34e355739944ba44
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58329316"
---
# <a name="teams-doesnt-launch"></a>Teams 未启动

如果尝试打开 Microsoft Teams 但它从未启动，请尝试以下操作：

1. 浏览到 **%appdata%\Microsoft\Teams**。
1. 删除文件夹的内容。
1. 重启计算机，然后尝试启动 Teams。

可能需要重新安装 Teams。要重新安装：

1. 使用控制面板卸载 Teams。
1. 浏览到 **%appdata%\Microsoft\Teams\Application Cache**。
1. 删除文件夹的内容。
1. 浏览到 **%appdata%\Microsoft\teams\Cache**。
1. 删除文件夹的内容。
1. 重新启动计算机，然后下载并安装 Teams。

如果要对无法登录的特定用户在租户上运行诊断，请使用关键字 **TeamsUserUnableToSignIn** 启动新的搜索，然后按照提示进行操作。