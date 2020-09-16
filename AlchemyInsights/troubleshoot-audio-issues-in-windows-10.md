---
title: 解决 Windows 10 中的音频问题
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750297"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a>解决 Windows 10 中的音频问题

**运行音频疑难解答**

1.  打开 " [疑难解答" 设置](ms-settings:troubleshoot)。

2.  选择 "**播放音频**  >  **" "运行疑难解答"**。

**设置默认设备**

如果使用 USB 或 HDMI 连接音频设备，则可能需要将该设备设置为默认设备：

1. 打开 **"启动**  >  **声音**"，然后从结果列表中选择 "**声音**" 或 "**更改系统声音**"。

2.  在 " **播放** " 选项卡上，选择一个设备，选择 " **设置默认值**"，然后选择 **"确定"**。

**检查电缆、音量、扬声器和耳机**

1. 检查您的扬声器和耳机连接是否有松动的电缆，并确保它们已连接到正确的插孔。

2. 检查电源和音量级别，并尝试打开所有音量控件。

3. 某些扬声器和应用程序具有自己的音量控制;您可能需要将它们全部签入，以确保它们处于正确的级别。

4. 尝试使用不同的 USB 端口进行连接。

**注意**：请记住，当耳机插入后，扬声器可能无法正常工作。

**检查设备管理器**

若要确保驱动程序是最新的，请执行以下操作：

1. 选择 " **开始**"，键入 " **设备管理器**"，然后从结果列表中选择 " **设备管理器** "。

2. 在 " **声音、视频和游戏控制器**" 下，选择您的声卡，打开它，选择 " **驱动因素** " 选项卡，然后选择 " **更新驱动程序**"。

**注意**：如果 Windows 找不到新的驱动程序，请在设备制造商的网站上查找一个驱动程序并按照其说明进行操作。

**重新安装驱动程序**

如果无法通过设备管理器进行更新或在制造商的网站上查找新的驱动程序，请尝试以下步骤：

1. 在 "设备管理器" 中，右键单击 (或长按) 音频驱动程序，然后选择 " **卸载**"。 重新启动设备，Windows 将尝试重新安装驱动程序。

2. 如果重新安装驱动程序不起作用，请尝试使用 Windows 附带的通用音频驱动程序。 在 "设备管理器" 中，右键单击 (或长按) 音频驱动程序 >**更新驱动程序软件**  >  **。若要**  >  **从 "我的电脑" 上的设备驱动程序列表**中选择 "我的电脑"，请选择 " **High Definition audio 设备**"，选择 "**下一步**"，然后按照说明安装它。
