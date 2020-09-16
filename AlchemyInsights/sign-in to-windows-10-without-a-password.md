---
title: 登录到 Windows 10，不使用密码
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 839b945c457cb007f13605c5b903ded75dadd1d7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47719943"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="7faa3-102">登录到 Windows 10，不使用密码</span><span class="sxs-lookup"><span data-stu-id="7faa3-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="7faa3-103">为了避免在 Windows 启动时必须键入密码，我们建议使用 Windows Hello 安全登录选项之一，如 PIN、面孔识别或指纹（如果可用）。</span><span class="sxs-lookup"><span data-stu-id="7faa3-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="7faa3-104">如果确实要禁用安全登录，请参阅下面的 "自动登录到 Windows 10" 说明。</span><span class="sxs-lookup"><span data-stu-id="7faa3-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="7faa3-105">**保护帐户密码的 Windows Hello 备选方案**</span><span class="sxs-lookup"><span data-stu-id="7faa3-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="7faa3-106">转[到 "](ms-settings:signinoptions?activationSource=GetHelp) **设置" > 帐户 > 登录选项**" (或单击") "。</span><span class="sxs-lookup"><span data-stu-id="7faa3-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="7faa3-107">将列出可用的登录选项。</span><span class="sxs-lookup"><span data-stu-id="7faa3-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="7faa3-108">例如：</span><span class="sxs-lookup"><span data-stu-id="7faa3-108">For example:</span></span>

![登录选项。](media/sign-in-options.png)

<span data-ttu-id="7faa3-110">单击或点击其中一个选项来对其进行配置。</span><span class="sxs-lookup"><span data-stu-id="7faa3-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="7faa3-111">下次启动或解锁 Windows 时，您将能够使用新选项而不是密码。</span><span class="sxs-lookup"><span data-stu-id="7faa3-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="7faa3-112">**自动登录到 Windows 10**</span><span class="sxs-lookup"><span data-stu-id="7faa3-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="7faa3-113">**注意**：自动登录非常方便，但会带来安全风险，尤其是当多人可以访问你的电脑时。</span><span class="sxs-lookup"><span data-stu-id="7faa3-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="7faa3-114">单击或点击任务栏中的 " **开始** " 按钮。</span><span class="sxs-lookup"><span data-stu-id="7faa3-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="7faa3-115">键入 **netplwiz** ，然后按 Enter 键打开 "用户帐户" 窗口。</span><span class="sxs-lookup"><span data-stu-id="7faa3-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="7faa3-116">在 " **用户帐户**" 中，单击 Windows 启动时要自动登录的帐户。</span><span class="sxs-lookup"><span data-stu-id="7faa3-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="7faa3-117">取消选中 "用户必须输入用户名和密码才能使用此计算机" 复选框。</span><span class="sxs-lookup"><span data-stu-id="7faa3-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![用户必须输入用户名和密码选项。](media/users-must-enter-username.png)

5. <span data-ttu-id="7faa3-119">单击\*\*\*\*“确定”。</span><span class="sxs-lookup"><span data-stu-id="7faa3-119">Click **OK**.</span></span> <span data-ttu-id="7faa3-120">系统将要求你输入并确认你选择的帐户的密码。</span><span class="sxs-lookup"><span data-stu-id="7faa3-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="7faa3-121">单击“确定”\*\*\*\* 完成。</span><span class="sxs-lookup"><span data-stu-id="7faa3-121">Click **OK** to finish.</span></span> <span data-ttu-id="7faa3-122">Windows 10 下次启动时，它将自动登录到您选择的帐户。</span><span class="sxs-lookup"><span data-stu-id="7faa3-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
