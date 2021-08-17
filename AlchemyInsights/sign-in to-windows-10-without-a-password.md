---
title: 使用密码Windows 10登录登录
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
ms.openlocfilehash: fbf190d433eabfee5b45348d05d918222a385314a431812aa5f5926aacf11560
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107496"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>使用密码Windows 10登录登录

为了避免在启动时键入密码Windows，我们建议你使用 Windows Hello 安全登录选项之一，如 PIN、人脸识别或指纹（如果可用）。 如果确实要禁用安全登录，请参阅下面的"自动登录Windows 10"说明。

**安全Windows Hello帐户密码的替代项**

转到设置 >**帐户>登录选项** ([或单击此处](ms-settings:signinoptions?activationSource=GetHelp)) 。 将列出可用的登录选项。 例如：

![登录选项。](media/sign-in-options.png)

单击或点击其中一个选项进行配置。 下次启动或解锁Windows时，你将可以使用新选项而不是密码。 

**自动登录Windows 10**

**注意**：自动登录很方便，但会带来安全风险，尤其是在电脑可供多个人访问时。 

1. 单击或点击 **任务栏中的** "开始"按钮。

2. 键入 **netplwiz 并** 按 Enter 键打开"用户帐户"窗口。

3. 在 **"用户帐户**"中，单击想要在启动帐户时自动Windows帐户。

4. 取消选中"用户必须输入用户名和密码才能使用此计算机"复选框。

    ![用户必须输入用户名和密码选项。](media/users-must-enter-username.png)

5. 单击“**确定**”。 系统将会要求你输入并确认所选帐户的密码。 单击“确定”完成。 下次Windows 10时，它将自动登录到所选的帐户。
