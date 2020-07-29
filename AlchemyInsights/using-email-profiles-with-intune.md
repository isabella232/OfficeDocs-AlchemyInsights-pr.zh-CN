---
title: 通过 Intune 使用电子邮件配置文件
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505181"
---
# <a name="using-email-profiles-with-intune"></a>通过 Intune 使用电子邮件配置文件

Intune 可用于在多个设备平台上为本机（内置）电子邮件客户端创建和部署电子邮件配置文件。

有关与电子邮件配置文件相关的某些限制的信息，包括如何处理现有配置文件的状态以及如何删除电子邮件配置文件，请参阅 [使用 Intune 将电子邮件设置添加到设备](https://docs.microsoft.com/intune/email-settings-configure)。

有关如何为每个设备平台创建电子邮件配置文件的更多信息，请参阅：

[用于在 Intune 中配置电子邮件、验证和同步的 Android 设备设置](https://docs.microsoft.com/intune/email-settings-android)  
[在 Microsoft Intune 中添加适用于 iOS 和 iPadOS 设备的电子邮件设置](https://docs.microsoft.com/intune/email-settings-ios)  
[适用于运行 Windows Phone 8.1 设备的 Microsoft Intune 电子邮件配置文件设置](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[适用于运行 Windows 10 设备的 Microsoft Intune 电子邮件配置文件设置](https://docs.microsoft.com/intune/email-settings-windows-10)

**常见同步问题**

**Android 电子邮件配置文件上的 KNOX 可阻止用户的联系人、日历和任务同步到用户设备。**

Android KNOX 电子邮件配置文件上的 KNOX 为管理员提供了一个选项，可以通过将每种内容类型都设置为“启用”来决定将哪些内容类型同步到设备。

如果将任何内容类型的设置设置为**未配置**（默认），则不会自动同步该内容类型。 用户可直接在设备上手动启用所需的内容类型，但该配置被 Intune 策略设置覆盖，同时该内容类型的同步停止。

