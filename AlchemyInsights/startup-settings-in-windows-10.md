---
title: Windows 10 中的启动设置
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828142"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="35acd-102">Windows 10 中的启动设置</span><span class="sxs-lookup"><span data-stu-id="35acd-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="35acd-103">**更改启动时自动运行的应用**</span><span class="sxs-lookup"><span data-stu-id="35acd-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="35acd-104">转到"[设置>应用>启动"。](ms-settings:startupapps?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="35acd-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="35acd-105">确保你想要在启动时运行的任何应用都处于打开 **。**</span><span class="sxs-lookup"><span data-stu-id="35acd-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="35acd-106">**添加应用以在启动时自动运行**</span><span class="sxs-lookup"><span data-stu-id="35acd-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="35acd-107">单击或点击 **"开始** "，找到想要在启动时运行的应用。</span><span class="sxs-lookup"><span data-stu-id="35acd-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="35acd-108">右键单击该应用 **，单击"** 更多"，然后单击"**打开文件位置"。**</span><span class="sxs-lookup"><span data-stu-id="35acd-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="35acd-109">这将打开保存应用快捷方式的位置。</span><span class="sxs-lookup"><span data-stu-id="35acd-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="35acd-110">如果没有"打开文件位置"选项，则意味着应用无法启动时运行。</span><span class="sxs-lookup"><span data-stu-id="35acd-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="35acd-111">打开文件位置后，按 Windows 徽标 **键 + R**，键入 **shell：startup**， **然后单击确定**。</span><span class="sxs-lookup"><span data-stu-id="35acd-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="35acd-112">这将打开"启动"文件夹。</span><span class="sxs-lookup"><span data-stu-id="35acd-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="35acd-113">将快捷方式从文件位置复制并粘贴到"启动"文件夹中。</span><span class="sxs-lookup"><span data-stu-id="35acd-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="35acd-114">**高级启动 (包括安全模式、UEFI 设置以及从另一台设备启动)**</span><span class="sxs-lookup"><span data-stu-id="35acd-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="35acd-115">保存工作并关闭所有打开的文档，因为这些步骤将重启电脑。</span><span class="sxs-lookup"><span data-stu-id="35acd-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="35acd-116">转到设置 [>更新&安全>恢复](ms-settings:recovery?activationSource=GetHelp)。</span><span class="sxs-lookup"><span data-stu-id="35acd-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="35acd-117">在 **"高级启动"** 下，单击 **"立即重新启动"。**</span><span class="sxs-lookup"><span data-stu-id="35acd-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="35acd-118">电脑重启到"选择选项"屏幕后：</span><span class="sxs-lookup"><span data-stu-id="35acd-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="35acd-119">若要从 USB 驱动器等设备启动，请单击 **"使用设备"。**</span><span class="sxs-lookup"><span data-stu-id="35acd-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="35acd-120">若要输入有时称为 BIOS (的 UEFI) ，请单击">**高级选项> UEFI 固件设置"。**</span><span class="sxs-lookup"><span data-stu-id="35acd-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="35acd-121">若要进入安全模式或更改高级启动设置，请单击">启动设置>高级选项 **疑难解答**"，然后单击"**重启"。**</span><span class="sxs-lookup"><span data-stu-id="35acd-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="35acd-122">系统可能会要求你输入 [BitLocker 恢复密钥](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)。</span><span class="sxs-lookup"><span data-stu-id="35acd-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="35acd-123">再次重启电脑后，单击想要使用的启动设置。</span><span class="sxs-lookup"><span data-stu-id="35acd-123">After your PC restarts again, click the startup setting you want to use.</span></span>