---
title: 在密码中使用指纹解锁Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: a171d889705a0035981465bdaa5a8f07b9d2eb7200ba4c948f2aaccbf2cc0a21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971877"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a>在密码中使用指纹解锁Windows 10

**启用Windows Hello指纹**

若要Windows 10指纹解锁指纹，你需要通过添加Windows Hello指纹 (让Windows至少一根手指) 指纹。 

1. 转到设置 >**帐户>登录选项** ([或单击此处](ms-settings:signinoptions?activationSource=GetHelp)) 。 将列出可用的登录选项。 例如：

    ![登录选项。](media/sign-in-options.png)

2. 单击或点击 **Windows Hello指纹**"，然后单击"**设置"。** 在"Windows Hello设置"窗口中，单击 **"开始使用"。** 指纹传感器将激活，并且你将被要求将手指放在传感器上：

   ![指纹传感器。](media/fingerprint-sensor.png)

3. 按照说明进行操作，这将要求你重复扫描手指。 完成此操作后，可以选择添加你可能想要用于登录的其他手指。 下次登录Windows 10，可以选择使用指纹进行登录。

**Windows Hello指纹无法作为登录选项使用**

如果Windows Hello指纹未显示为登录选项中的选项，则意味着Windows 无法识别附加到电脑的任何指纹读取器/扫描仪，或者如果例如，你的电脑由工作区) 管理，则系统策略会阻止其使用 (。 疑难解答： 

1. 选择 **任务栏中的** "开始"按钮，然后搜索 **设备管理器**。

2. 单击或点击打开 **设备管理器**。

3. 在设备管理器中，通过单击其 V 号展开生物识别设备。

   ![生物识别设备。](media/biometric-devices.png)

4. 指纹扫描仪应列为生物识别设备，如 Synaptics WBDI 扫描仪：

   ![生物识别设备。](media/biometric-devices-expanded.png)

5. 如果未显示指纹扫描仪，并且扫描仪已集成到电脑中，请转到电脑制造商的网站。 在电脑型号的技术支持部分，搜索Windows 10可安装的扫描仪的驱动程序。

6. 如果扫描仪与通过 USB (连接的电脑驱动器) ，请转到扫描仪制造商的网站，查找并安装适用于扫描仪型号的 Windows 10 设备驱动程序软件。
