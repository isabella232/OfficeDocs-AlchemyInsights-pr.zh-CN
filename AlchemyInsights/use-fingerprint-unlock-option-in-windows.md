---
title: 在 Windows 10 中使用指纹解锁选项
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795234"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="3f526-102">在 Windows 10 中使用指纹解锁选项</span><span class="sxs-lookup"><span data-stu-id="3f526-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="3f526-103">**启用 Windows Hello 指纹**</span><span class="sxs-lookup"><span data-stu-id="3f526-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="3f526-104">若要使用你的指纹解锁 Windows 10，你需要通过添加 (让 Windows 了解至少在一根手指中识别) ，从而设置 Windows Hello 指纹。</span><span class="sxs-lookup"><span data-stu-id="3f526-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="3f526-105">转[到 "](ms-settings:signinoptions?activationSource=GetHelp) **设置" > 帐户 > 登录选项**" (或单击") "。</span><span class="sxs-lookup"><span data-stu-id="3f526-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="3f526-106">将列出可用的登录选项。</span><span class="sxs-lookup"><span data-stu-id="3f526-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="3f526-107">例如：</span><span class="sxs-lookup"><span data-stu-id="3f526-107">For example:</span></span>

    ![登录选项。](media/sign-in-options.png)

2. <span data-ttu-id="3f526-109">单击或点击 " **Windows Hello 指纹**"，然后单击 " **设置**"。</span><span class="sxs-lookup"><span data-stu-id="3f526-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="3f526-110">在 "Windows Hello 安装程序" 窗口中，单击 " **开始**"。</span><span class="sxs-lookup"><span data-stu-id="3f526-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="3f526-111">指纹传感器将激活，系统将要求你将手指放在传感器上：</span><span class="sxs-lookup"><span data-stu-id="3f526-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![指纹传感器。](media/fingerprint-sensor.png)

3. <span data-ttu-id="3f526-113">按照说明操作，这将要求您反复扫描手指。</span><span class="sxs-lookup"><span data-stu-id="3f526-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="3f526-114">完成此操作后，你可以选择添加其他可能要用于登录的手指。</span><span class="sxs-lookup"><span data-stu-id="3f526-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="3f526-115">下次登录到 Windows 10 时，你可以选择使用你的指纹执行此操作。</span><span class="sxs-lookup"><span data-stu-id="3f526-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="3f526-116">**Windows Hello 指纹不可用作登录选项**</span><span class="sxs-lookup"><span data-stu-id="3f526-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="3f526-117">如果 Windows Hello 指纹不显示为 **登录选项**中的选项，则说明 windows 不知道连接到电脑的任何指纹读取器/扫描程序，或者系统策略阻止其使用 (如果你的电脑由你的工作环境管理) 。</span><span class="sxs-lookup"><span data-stu-id="3f526-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="3f526-118">若要解决此问题：</span><span class="sxs-lookup"><span data-stu-id="3f526-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="3f526-119">选择任务栏中的 " **开始** " 按钮，并搜索 " **设备管理器**"。</span><span class="sxs-lookup"><span data-stu-id="3f526-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="3f526-120">单击或点击以打开 " **设备管理器**"。</span><span class="sxs-lookup"><span data-stu-id="3f526-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="3f526-121">在设备管理器中，单击 "生物" 设备的 v 形展开。</span><span class="sxs-lookup"><span data-stu-id="3f526-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![生物识别设备。](media/biometric-devices.png)

4. <span data-ttu-id="3f526-123">您的指纹扫描器应作为生物识别设备（如 Synaptics WBDI 扫描程序）列出：</span><span class="sxs-lookup"><span data-stu-id="3f526-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![生物识别设备。](media/biometric-devices-expanded.png)

5. <span data-ttu-id="3f526-125">如果你的指纹扫描器未显示，并且已将扫描仪集成到你的电脑中，请转到电脑制造商的网站。</span><span class="sxs-lookup"><span data-stu-id="3f526-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="3f526-126">在电脑模型的 "技术支持" 部分，搜索可安装的扫描仪的 Windows 10 驱动程序。</span><span class="sxs-lookup"><span data-stu-id="3f526-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="3f526-127">如果扫描仪与电脑 (通过 USB) 相连，请转到扫描仪制造商的网站，查找并安装适用于扫描仪模型的 Windows 10 设备驱动程序软件。</span><span class="sxs-lookup"><span data-stu-id="3f526-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
