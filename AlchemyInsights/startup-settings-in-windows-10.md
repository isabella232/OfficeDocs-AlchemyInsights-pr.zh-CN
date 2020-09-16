---
title: Windows 10 中的启动设置
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751125"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="17a47-102">Windows 10 中的启动设置</span><span class="sxs-lookup"><span data-stu-id="17a47-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="17a47-103">**更改启动时自动运行的应用程序**</span><span class="sxs-lookup"><span data-stu-id="17a47-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="17a47-104">转到 " [设置" > 应用程序 > 启动](ms-settings:startupapps?activationSource=GetHelp)"。</span><span class="sxs-lookup"><span data-stu-id="17a47-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="17a47-105">请确保启用了要在启动时运行的任何应用**程序。**</span><span class="sxs-lookup"><span data-stu-id="17a47-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="17a47-106">**添加在启动时自动运行的应用程序**</span><span class="sxs-lookup"><span data-stu-id="17a47-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="17a47-107">单击或点击 " **启动** "，并查找要在启动时运行的应用程序。</span><span class="sxs-lookup"><span data-stu-id="17a47-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="17a47-108">右键单击该应用程序，单击 " **更多**"，然后单击 " **打开文件位置**"。</span><span class="sxs-lookup"><span data-stu-id="17a47-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="17a47-109">这将打开保存应用程序的快捷方式的位置。</span><span class="sxs-lookup"><span data-stu-id="17a47-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="17a47-110">如果打开文件位置没有任何选项，则表示该应用程序在启动时无法运行。</span><span class="sxs-lookup"><span data-stu-id="17a47-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="17a47-111">打开文件位置，按 **Windows 徽标键 + R**，键入 **shell： startup**，然后单击 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="17a47-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="17a47-112">这将打开 "启动" 文件夹。</span><span class="sxs-lookup"><span data-stu-id="17a47-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="17a47-113">将文件位置的应用程序的快捷方式复制并粘贴到启动文件夹。</span><span class="sxs-lookup"><span data-stu-id="17a47-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="17a47-114">\*\*高级启动选项 (包括安全模式、UEFI 设置和从其他设备启动) \*\*</span><span class="sxs-lookup"><span data-stu-id="17a47-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="17a47-115">保存您的工作并关闭任何打开的文档，因为这些步骤将重新启动电脑。</span><span class="sxs-lookup"><span data-stu-id="17a47-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="17a47-116">转到 " [设置" > 更新 & 安全 > 恢复](ms-settings:recovery?activationSource=GetHelp)。</span><span class="sxs-lookup"><span data-stu-id="17a47-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="17a47-117">在 " **高级启动**" 下，单击 " **立即重新启动**"。</span><span class="sxs-lookup"><span data-stu-id="17a47-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="17a47-118">在电脑重新启动到 "选择选项" 屏幕之后：</span><span class="sxs-lookup"><span data-stu-id="17a47-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="17a47-119">若要从 USB 驱动器之类的设备进行引导，请单击 " **使用设备**"。</span><span class="sxs-lookup"><span data-stu-id="17a47-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="17a47-120">若要输入 UEFI 设置 (有时称为 BIOS 设置) ，请单击 " **疑难解答" > 高级选项 > UEFI 固件设置**。</span><span class="sxs-lookup"><span data-stu-id="17a47-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="17a47-121">若要进入安全模式或更改高级启动设置，请单击 " **疑难解答" > 高级选项 "> 启动设置**"，然后单击 " **重新启动**"。</span><span class="sxs-lookup"><span data-stu-id="17a47-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="17a47-122">系统可能会要求你输入 [BitLocker 恢复密钥](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)。</span><span class="sxs-lookup"><span data-stu-id="17a47-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="17a47-123">电脑再次重新启动后，单击要使用的启动设置。</span><span class="sxs-lookup"><span data-stu-id="17a47-123">After your PC restarts again, click the startup setting you want to use.</span></span>