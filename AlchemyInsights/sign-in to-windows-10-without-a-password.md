---
title: 登录到 Windows 10，不使用密码
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588271"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>登录到 Windows 10，不使用密码

为了避免在 Windows 启动时必须键入密码，我们建议使用 Windows Hello 安全登录选项之一，如 PIN、面孔识别或指纹（如果可用）。 如果确实要禁用安全登录，请参阅下面的 "自动登录到 Windows 10" 说明。

**保护帐户密码的 Windows Hello 备选方案**

转到 "**设置" > 帐户 > 登录选项**（或单击[此处](ms-settings:signinoptions?activationSource=GetHelp)）。 将列出可用的登录选项。 例如：

![登录选项。](media/sign-in-options.png)

单击或点击其中一个选项来对其进行配置。 下次启动或解锁 Windows 时，您将能够使用新选项而不是密码。 

**自动登录到 Windows 10**

**注意**：自动登录非常方便，但会带来安全风险，尤其是当多人可以访问你的电脑时。 

1. 单击或点击任务栏中的 "**开始**" 按钮。

2. 键入**netplwiz** ，然后按 Enter 键打开 "用户帐户" 窗口。

3. 在 "**用户帐户**" 中，单击 Windows 启动时要自动登录的帐户。

4. 取消选中 "用户必须输入用户名和密码才能使用此计算机" 复选框。

    ![用户必须输入用户名和密码选项。](media/users-must-enter-username.png)

5. 单击 **“确定”**。 系统将要求你输入并确认你选择的帐户的密码。 单击“确定”**** 完成。 Windows 10 下次启动时，它将自动登录到您选择的帐户。
