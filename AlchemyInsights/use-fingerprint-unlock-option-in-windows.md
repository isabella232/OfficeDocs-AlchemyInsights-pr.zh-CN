---
title: 在 Windows 10 中使用指纹解锁选项
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588306"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>在 Windows 10 中使用指纹解锁选项

**启用 Windows Hello 指纹**

若要使用你的指纹解锁 Windows 10，你需要通过添加（让 Windows 学习识别）至少一个手指来设置 Windows Hello 指纹。 

1. 转到 "**设置" > 帐户 > 登录选项**（或单击[此处](ms-settings:signinoptions?activationSource=GetHelp)）。 将列出可用的登录选项。 例如：

    ![登录选项。](media/sign-in-options.png)

2. 单击或点击 " **Windows Hello 指纹**"，然后单击 "**设置**"。 在 "Windows Hello 安装程序" 窗口中，单击 "**开始**"。 指纹传感器将激活，系统将要求你将手指放在传感器上：

   ![指纹传感器。](media/fingerprint-sensor.png)

3. 按照说明操作，这将要求您反复扫描手指。 完成此操作后，你可以选择添加其他可能要用于登录的手指。 下次登录到 Windows 10 时，你可以选择使用你的指纹执行此操作。

**Windows Hello 指纹不可用作登录选项**

如果 Windows Hello 指纹不显示为**登录选项**中的选项，则说明 windows 不知道连接到你的电脑的任何指纹读取器/扫描程序，或者系统策略阻止其使用（如果你的电脑由你的工作环境管理）。 若要解决此问题： 

1. 选择任务栏中的 "**开始**" 按钮，并搜索 "**设备管理器**"。

2. 单击或点击以打开 "**设备管理器**"。

3. 在设备管理器中，单击 "生物" 设备的 v 形展开。

   ![生物识别设备。](media/biometric-devices.png)

4. 您的指纹扫描器应作为生物识别设备（如 Synaptics WBDI 扫描程序）列出：

   ![生物识别设备。](media/biometric-devices-expanded.png)

5. 如果你的指纹扫描器未显示，并且已将扫描仪集成到你的电脑中，请转到电脑制造商的网站。 在电脑模型的 "技术支持" 部分，搜索可安装的扫描仪的 Windows 10 驱动程序。

6. 如果扫描仪与电脑（通过 USB 连接）不同，请转到扫描仪制造商的网站，查找并安装适用于您的扫描仪模型的 Windows 10 设备驱动程序软件。
