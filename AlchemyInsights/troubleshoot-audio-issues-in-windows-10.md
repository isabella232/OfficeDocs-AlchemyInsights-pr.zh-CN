---
title: 解决 Windows 10 中的音频问题
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750297"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="ae728-102">解决 Windows 10 中的音频问题</span><span class="sxs-lookup"><span data-stu-id="ae728-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="ae728-103">**运行音频疑难解答**</span><span class="sxs-lookup"><span data-stu-id="ae728-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="ae728-104">打开 " [疑难解答" 设置](ms-settings:troubleshoot)。</span><span class="sxs-lookup"><span data-stu-id="ae728-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="ae728-105">选择 "**播放音频**  >  **" "运行疑难解答"**。</span><span class="sxs-lookup"><span data-stu-id="ae728-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="ae728-106">**设置默认设备**</span><span class="sxs-lookup"><span data-stu-id="ae728-106">**Set the default device**</span></span>

<span data-ttu-id="ae728-107">如果使用 USB 或 HDMI 连接音频设备，则可能需要将该设备设置为默认设备：</span><span class="sxs-lookup"><span data-stu-id="ae728-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="ae728-108">打开 **"启动**  >  **声音**"，然后从结果列表中选择 "**声音**" 或 "**更改系统声音**"。</span><span class="sxs-lookup"><span data-stu-id="ae728-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="ae728-109">在 " **播放** " 选项卡上，选择一个设备，选择 " **设置默认值**"，然后选择 **"确定"**。</span><span class="sxs-lookup"><span data-stu-id="ae728-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="ae728-110">**检查电缆、音量、扬声器和耳机**</span><span class="sxs-lookup"><span data-stu-id="ae728-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="ae728-111">检查您的扬声器和耳机连接是否有松动的电缆，并确保它们已连接到正确的插孔。</span><span class="sxs-lookup"><span data-stu-id="ae728-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="ae728-112">检查电源和音量级别，并尝试打开所有音量控件。</span><span class="sxs-lookup"><span data-stu-id="ae728-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="ae728-113">某些扬声器和应用程序具有自己的音量控制;您可能需要将它们全部签入，以确保它们处于正确的级别。</span><span class="sxs-lookup"><span data-stu-id="ae728-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="ae728-114">尝试使用不同的 USB 端口进行连接。</span><span class="sxs-lookup"><span data-stu-id="ae728-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="ae728-115">**注意**：请记住，当耳机插入后，扬声器可能无法正常工作。</span><span class="sxs-lookup"><span data-stu-id="ae728-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="ae728-116">**检查设备管理器**</span><span class="sxs-lookup"><span data-stu-id="ae728-116">**Check Device Manager**</span></span>

<span data-ttu-id="ae728-117">若要确保驱动程序是最新的，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="ae728-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="ae728-118">选择 " **开始**"，键入 " **设备管理器**"，然后从结果列表中选择 " **设备管理器** "。</span><span class="sxs-lookup"><span data-stu-id="ae728-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="ae728-119">在 " **声音、视频和游戏控制器**" 下，选择您的声卡，打开它，选择 " **驱动因素** " 选项卡，然后选择 " **更新驱动程序**"。</span><span class="sxs-lookup"><span data-stu-id="ae728-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="ae728-120">**注意**：如果 Windows 找不到新的驱动程序，请在设备制造商的网站上查找一个驱动程序并按照其说明进行操作。</span><span class="sxs-lookup"><span data-stu-id="ae728-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="ae728-121">**重新安装驱动程序**</span><span class="sxs-lookup"><span data-stu-id="ae728-121">**Reinstall the driver**</span></span>

<span data-ttu-id="ae728-122">如果无法通过设备管理器进行更新或在制造商的网站上查找新的驱动程序，请尝试以下步骤：</span><span class="sxs-lookup"><span data-stu-id="ae728-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="ae728-123">在 "设备管理器" 中，右键单击 (或长按) 音频驱动程序，然后选择 " **卸载**"。</span><span class="sxs-lookup"><span data-stu-id="ae728-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="ae728-124">重新启动设备，Windows 将尝试重新安装驱动程序。</span><span class="sxs-lookup"><span data-stu-id="ae728-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="ae728-125">如果重新安装驱动程序不起作用，请尝试使用 Windows 附带的通用音频驱动程序。</span><span class="sxs-lookup"><span data-stu-id="ae728-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="ae728-126">在 "设备管理器" 中，右键单击 (或长按) 音频驱动程序 >**更新驱动程序软件**  >  **。若要**  >  **从 "我的电脑" 上的设备驱动程序列表**中选择 "我的电脑"，请选择 " **High Definition audio 设备**"，选择 "**下一步**"，然后按照说明安装它。</span><span class="sxs-lookup"><span data-stu-id="ae728-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
