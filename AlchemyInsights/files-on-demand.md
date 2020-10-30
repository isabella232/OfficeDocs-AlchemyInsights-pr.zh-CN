---
title: 文件随选
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 4e3da81ee048c6257e05b998c0f457fa433738fd
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791284"
---
# <a name="configure-files-on-demand"></a>配置文件随选

“文件随选”需要 [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040)（版本 1709 或更高版本）或 WIndows Server 2019 和 OneDrive 内部版本 17.3.7064.1005 或更高版本。

OneDrive 文件随选可帮助访问 OneDrive 中的所有文件，而无需下载所有这些文件和使用设备上的存储空间。

要在电脑上配置文件随选，请执行以下操作：

1. 选择Windows任务栏通知区域中的白色或蓝色 **OneDrive** 云图标。 选择 **帮助 & "设置** 齿轮图标 > **设置s** 。
2. 在“ **设置** ”选项卡上，选中“ **节省空间并在需要使用时下载文件** ”复选框。  

还可以使用注册表配置文件随选。

如果禁用此设置，Windows 10 用户的同步行为会与旧版 Windows 用户相同，并且无法启用文件随选。 如果未配置此选项，则用户可以打开或关闭文件随选。

启用此策略会将下面的注册表项值设置为 1。 禁用此策略会将以下注册表键值设置为0。

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

如果您在 "设置 "中看不到 "随选文件 "选项，请确保 "Windows Cloud Files Filter Driver "服务的启动类型设置为 2 (AUTO_START)。 启用此功能会将以下注册表键值设置为2。

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`