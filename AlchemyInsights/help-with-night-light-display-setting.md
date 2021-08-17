---
title: 有关夜灯显示设置的帮助
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: 7da8d4cefe2140340892544d73b9f8e3f3fdc679e9d58f2ad5ac12bf30830c5c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54078708"
---
# <a name="help-with-the-night-light-display-setting"></a>有关夜灯显示设置的帮助

若要深入了解夜灯显示设置，请参阅 [在 Windows 10 设备夜间显示](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)。

如果"设置"中夜灯选项灰显，请检查显示驱动程序： 

1. 点击任务栏的搜索框，键入 **设备管理器**，然后从搜索结果中选择 **设备管理器**。
1. 展开 **显示适配器**。 

遗憾的是，如果你的设备使用 DisplayLink 驱动程序或基本显示驱动程序，则夜灯功能不可用。

夜灯功能利用最新的图形技术，因此你可能需要更新显示驱动程序：  

- 若要检查更新，请转到 **开始** > **设置** > **更新与安全** > **Windows 更新** > **检查更新**。  

或

- 访问硬件制造商的支持网站，手动下载并安装最新的显示驱动程序。

## <a name="reset-night-light-in-the-registry"></a>在注册表中重置夜灯

如果更新显示驱动程序不起作用，则可能需要在注册表中重置夜灯。  

**注意：** 建议仅向高级用户提供此疑难解答步骤。 如果注册表修改不当，可能会出现严重问题。 为增强保护，请在修改前备份注册表，以便出现问题时可以还原。

1. 在搜索框中，键入 **regedit**，然后在搜索结果中选择 **注册表编辑器**。

1. 转到下面的注册表项： 

    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount

1. 导出并删除以下子项：$$windows.data.bluelightreduction.bluelightreductionstate

1. 导出并删除以下子项：$$windows.data.bluelightreduction.settings

1. 重启 Windows，验证夜灯选项是否可用。


