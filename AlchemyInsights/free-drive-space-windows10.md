---
title: 在 Windows 10 中释放驱动器空间
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: c7d29ab718be8dbdcde61a7de2f158fb3bbd722d2964d8b13cde9936dd1e5ee1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928071"
---
# <a name="free-up-drive-space-in-windows-10"></a>在 Windows 10 中释放驱动器空间

以下是在 Windows 中释放驱动器空间的两个选项：

- 在 Windows 10 中释放驱动器空间。
- 通过外部存储设备为 Windows 10 更新释放空间。

如果使用“磁盘清理”后，磁盘空间仍然不足，则你的 Temp 文件夹可能很快就会被 Microsoft Store 使用的应用程序 (.appx) 文件填满。 若要修复此问题，请重置 Microsoft Store，清除 Microsoft Store 缓存，然后运行 Windows Update 故障排除程序。 在继续执行这些步骤之前，请确保 Microsoft Store 已关闭。

**步骤 1：重置 Microsoft Store**

**注意** 这将永久删除设备上的应用数据，包括首选项和登录详细信息。

1. 选择“**开始**” > “**设置**” > “**应用**” > “**应用和功能**”。

1. 在应用列表中，找到并选择“Microsoft Store”。

1. 选择“**高级选项**”。

1. 向下滚动并选择“**重置**”，然后选择“**确认重置**”。

**步骤 2：清除 Microsoft Store 缓存**

1. 按 Windows 徽标键 + R 以打开“运行”对话框。

1. 键入 wsreset.exe，然后选择“**确定**”。

1. 此时会打开一个空白的命令提示符窗口。 约 10 秒钟后，窗口将关闭并自动打开 Microsoft Store。

**步骤 3：重置 Windows 更新**

1. 选择“**开始**” > “**设置**” > “**更新和安全**” > “**故障排除**”。

1. 向下滚动并从列表中选择“**Windows 更新**”，然后选择“**运行故障排除程序**”。

1. 重新启动计算机，检查是否仍遇到此问题。

