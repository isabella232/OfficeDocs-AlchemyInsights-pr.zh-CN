---
title: 使用 TeamViewer 远程管理 Intune 设备
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
- "1284"
- "6700008"
ms.openlocfilehash: e931b2092ab049bc01c600344cbd4702848abcd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798438"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>使用 TeamViewer 远程管理 Intune 设备

可使用 [TeamViewer](https://www.teamviewer.com/) 远程管理由 Intune 管理的设备。

若要使用 TeamViewer 管理 Intune，请使用以下步骤： 

首先从 TeamViewer 获取凭据，以在 Intune 上设置 TeamViewer 连接器。 这允许管理员在“设备”下的 TeamViewer 连接器用户界面中输入凭据，这是一项一次性操作，用于在 Intune 和 TeamViewer 服务之间建立关联。

**第 1 部分：使用远程设备启动会话**

1. 在“**所有设备**”下，选择要用来启动远程会话的设备。
2. 从 **…更多**中，选择“**新建远程协助会话**”。
3. 选择“**是**”可确认你想要建立远程会话。
    TeamViewer 服务确认“启动新远程会话”请求后，将在设备概述（或 Essentials）窗格的详细信息中看到“**启动远程协助**”选项。 选择“**查看更多**”以展开窗格并显示“远程协助”状态。
4. 选择“**启动远程会话**”以在管理员端启动会话。
5. 选择下载 TeamViewer 二进制文件（Windows），然后选择“**运行**”。<br/>
    **注意**可以忽略打开到 TeamViewer 网站的任何 Web 浏览器页面。

6. 确认对 TeamViewer 应用的请求，以便在设备上进行更改（仅限 Windows）。
7. TeamViewer 应用程序启动并包含用于验证与远程设备的连接的会话代码。

**第 2 部分：在面向远程会话的设备上**

1. 打开 Intune 公司门户。
2. 查找通知标志：“你的 IT 管理员正在请求控制此设备的远程协助会话”，然后选择通知。
3. 选择下载 TeamViewer 应用程序，或者从 app store 中确认下载 TeamViewer 应用，然后选择“**运行**”。
    **注意**可以忽略打开到 TeamViewer 网站的任何 Web 浏览器页面。

4. 确认对 TeamViewer 应用的请求，以便在设备上进行更改（仅限 Windows）。
5. TeamViewer 应用程序启动并包含用于验证与远程设备的连接的会话代码。
6. 弹出窗口询问是否要允许开始会话。

**注意**由 TeamViewer 服务生成的会话代码仅供一次性使用。 如果失去连接，则必须：

1. 关闭远程设备和管理工作站上的 TeamViewer 应用程序实例。
2. 关闭远程设备上的公司门户。
3. 从管理门户启动一个新的 "新建远程协助会话"。
4. 重新打开远程设备上的公司门户以接收新的通知。
5. 与以前一样，在远程设备和管理工作站上下载并打开 TeamViewer 应用程序。