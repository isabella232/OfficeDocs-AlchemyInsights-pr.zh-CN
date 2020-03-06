---
title: Windows 10 中的启动设置
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: b4854944d8cbd9bd83fdea609007c15d39c8eb75
ms.sourcegitcommit: c55eea624d960d2dd17ac4aa5a4c23e34e6443b8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2020
ms.locfileid: "42408931"
---
# <a name="startup-settings-in-windows-10"></a>Windows 10 中的启动设置

**更改启动时自动运行的应用程序**

1. 转到 "[设置" > 应用程序 > 启动](ms-settings:startupapps?activationSource=GetHelp)"。

2. 请确保启用了要在启动时运行的任何应用**程序。**

**添加在启动时自动运行的应用程序**

1. 单击或点击 "**启动**"，并查找要在启动时运行的应用程序。

2. 右键单击该应用程序，单击 "**更多**"，然后单击 "**打开文件位置**"。 这将打开保存应用程序的快捷方式的位置。 如果打开文件位置没有任何选项，则表示该应用程序在启动时无法运行。

3. 打开文件位置，按**Windows 徽标键 + R**，键入**shell： startup**，然后单击 **"确定"**。 这将打开 "启动" 文件夹。

4. 将文件位置的应用程序的快捷方式复制并粘贴到启动文件夹。

**高级启动选项（包括安全模式、UEFI 设置和从其他设备启动）**

1. 保存您的工作并关闭任何打开的文档，因为这些步骤将重新启动电脑。

2. 转到 "[设置" > 更新 & 安全 > 恢复](ms-settings:recovery?activationSource=GetHelp)。

3. 在 "**高级启动**" 下，单击 "**立即重新启动**"。 

4. 在电脑重新启动到 "选择选项" 屏幕之后：

    - 若要从 USB 驱动器之类的设备进行引导，请单击 "**使用设备**"。

    - 若要输入 UEFI 设置（有时称为 BIOS 设置），请单击 " **> 高级选项" 的 "疑难解答" > UEFI 固件设置**。 

    - 若要进入安全模式或更改高级启动设置，请单击 "**疑难解答" > 高级选项 "> 启动设置**"，然后单击 "**重新启动**"。 系统可能会要求你输入[BitLocker 恢复密钥](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)。 电脑再次重新启动后，单击要使用的启动设置。