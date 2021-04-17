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
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="0e1de-102">无需使用密码即可登录 Windows 10</span><span class="sxs-lookup"><span data-stu-id="0e1de-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="0e1de-103">为了避免在 Windows 启动时键入密码，我们建议你使用 Windows Hello 安全登录选项之一，如 PIN、人脸识别或指纹（如果可用）。</span><span class="sxs-lookup"><span data-stu-id="0e1de-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="0e1de-104">如果确实要禁用安全登录，请参阅下面的"自动登录 Windows 10"说明。</span><span class="sxs-lookup"><span data-stu-id="0e1de-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="0e1de-105">**保护帐户密码的 Windows Hello 替代项**</span><span class="sxs-lookup"><span data-stu-id="0e1de-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="0e1de-106">转到设置 **>帐户>登录选项** ([或单击此处](ms-settings:signinoptions?activationSource=GetHelp)) 。</span><span class="sxs-lookup"><span data-stu-id="0e1de-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="0e1de-107">将列出可用的登录选项。</span><span class="sxs-lookup"><span data-stu-id="0e1de-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="0e1de-108">例如：</span><span class="sxs-lookup"><span data-stu-id="0e1de-108">For example:</span></span>

![登录选项。](media/sign-in-options.png)

<span data-ttu-id="0e1de-110">单击或点击其中一个选项进行配置。</span><span class="sxs-lookup"><span data-stu-id="0e1de-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="0e1de-111">下次启动或解锁 Windows 时，你将可以使用新选项而不是密码。</span><span class="sxs-lookup"><span data-stu-id="0e1de-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="0e1de-112">**自动登录 Windows 10**</span><span class="sxs-lookup"><span data-stu-id="0e1de-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="0e1de-113">**注意**：自动登录很方便，但会带来安全风险，尤其是在电脑可供多个人访问时。</span><span class="sxs-lookup"><span data-stu-id="0e1de-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="0e1de-114">单击或点击 **任务栏中的** "开始"按钮。</span><span class="sxs-lookup"><span data-stu-id="0e1de-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="0e1de-115">键入 **netplwiz 并** 按 Enter 键打开"用户帐户"窗口。</span><span class="sxs-lookup"><span data-stu-id="0e1de-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="0e1de-116">在 **用户帐户** 中，单击你想要在 Windows 启动时自动登录的帐户。</span><span class="sxs-lookup"><span data-stu-id="0e1de-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="0e1de-117">取消选中"用户必须输入用户名和密码才能使用此计算机"复选框。</span><span class="sxs-lookup"><span data-stu-id="0e1de-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![用户必须输入用户名和密码选项。](media/users-must-enter-username.png)

5. <span data-ttu-id="0e1de-119">单击“**确定**”。</span><span class="sxs-lookup"><span data-stu-id="0e1de-119">Click **OK**.</span></span> <span data-ttu-id="0e1de-120">系统将会要求你输入并确认所选帐户的密码。</span><span class="sxs-lookup"><span data-stu-id="0e1de-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="0e1de-121">单击“确定”完成。</span><span class="sxs-lookup"><span data-stu-id="0e1de-121">Click **OK** to finish.</span></span> <span data-ttu-id="0e1de-122">下次 Windows 10 启动时，它将自动登录到你选择的帐户。</span><span class="sxs-lookup"><span data-stu-id="0e1de-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
