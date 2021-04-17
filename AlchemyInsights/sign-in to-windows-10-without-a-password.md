---
title: 无需使用密码即可登录 Windows 10
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830536"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>无需使用密码即可登录 Windows 10

为了避免在 Windows 启动时键入密码，我们建议你使用 Windows Hello 安全登录选项之一，如 PIN、人脸识别或指纹（如果可用）。 如果确实要禁用安全登录，请参阅下面的"自动登录 Windows 10"说明。

**保护帐户密码的 Windows Hello 替代项**

转到设置 **>帐户>登录选项** ([或单击此处](ms-settings:signinoptions?activationSource=GetHelp)) 。 将列出可用的登录选项。 例如：

![登录选项。](media/sign-in-options.png)

单击或点击其中一个选项进行配置。 下次启动或解锁 Windows 时，你将可以使用新选项而不是密码。 

**自动登录 Windows 10**

**注意**：自动登录很方便，但会带来安全风险，尤其是在电脑可供多个人访问时。 

1. 单击或点击 **任务栏中的** "开始"按钮。

2. 键入 **netplwiz 并** 按 Enter 键打开"用户帐户"窗口。

3. 在 **用户帐户** 中，单击你想要在 Windows 启动时自动登录的帐户。

4. 取消选中"用户必须输入用户名和密码才能使用此计算机"复选框。

    ![用户必须输入用户名和密码选项。](media/users-must-enter-username.png)

5. 单击“**确定**”。 系统将会要求你输入并确认所选帐户的密码。 单击“确定”完成。 下次 Windows 10 启动时，它将自动登录到你选择的帐户。
