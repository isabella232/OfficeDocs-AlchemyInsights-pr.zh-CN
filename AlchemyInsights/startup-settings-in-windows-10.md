---
title: Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909816"
---
# <a name="startup-settings-in-windows-10"></a>Windows 10

**更改启动时自动运行的应用**

1. 转到["设置 >应用>启动"。](ms-settings:startupapps?activationSource=GetHelp)

2. 确保你想要在启动时运行的任何应用都处于打开 **。**

**添加应用以在启动时自动运行**

1. 单击或点击 **"开始** "，找到想要在启动时运行的应用。

2. 右键单击该应用 **，单击"** 更多"，然后单击"**打开文件位置"。** 这将打开保存应用快捷方式的位置。 如果没有"打开文件位置"选项，则意味着应用无法启动时运行。

3. 打开文件位置后，按 **Windows键 + R，** 键入 **shell：startup**，**然后单击确定。** 这将打开"启动"文件夹。

4. 将快捷方式从文件位置复制并粘贴到"启动"文件夹中。

**高级启动选项 (包括保险箱模式、UEFI 设置以及从另一台设备启动)**

1. 保存工作并关闭所有打开的文档，因为这些步骤将重启电脑。

2. 转到["设置 >更新&安全>恢复"。](ms-settings:recovery?activationSource=GetHelp)

3. 在 **"高级启动"** 下，单击 **"立即重新启动"。** 

4. 电脑重启到"选择选项"屏幕后：

    - 若要从 USB 驱动器等设备启动，请单击 **"使用设备"。**

    - 若要输入有时称为 BIOS (的 UEFI 设置) ，请单击"> **UEFI** 固件>高级选项设置。 

    - 若要输入保险箱模式或更改高级启动设置，请单击">启动>高级设置 **疑** 难解答"，然后单击"重启 **"。** 系统可能会要求你输入 [BitLocker 恢复密钥](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)。 再次重启电脑后，单击想要使用的启动设置。