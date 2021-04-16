---
title: Windows 10 中缺少电源或电池图标
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790538"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="4e20d-102">Windows 10 中缺少电源或电池图标</span><span class="sxs-lookup"><span data-stu-id="4e20d-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="4e20d-103">如果你的 Windows 10 设备装有电池（例如，笔记本电脑或平板电脑或者通过 USB 连接到 UPS 的电脑），则通常会在任务栏上的时钟附近显示电源/电池图标，例如：</span><span class="sxs-lookup"><span data-stu-id="4e20d-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![电池图标](media/battery-icon.png)

<span data-ttu-id="4e20d-105">如果看不到此图标，则它可能处于隐藏状态：</span><span class="sxs-lookup"><span data-stu-id="4e20d-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="4e20d-106">转到“**[设置”>“个性化”>“任务栏](ms-settings:taskbar?activationSource=GetHelp)**”。</span><span class="sxs-lookup"><span data-stu-id="4e20d-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="4e20d-107">在通知区域中，单击“**选择在任务栏上显示哪些图标**”。</span><span class="sxs-lookup"><span data-stu-id="4e20d-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="4e20d-108">然后在列表中查找“**电源**”项，并将其设置切换为“**打开**”。</span><span class="sxs-lookup"><span data-stu-id="4e20d-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![在任务栏中显示电源图标](media/power-icon-on.png)

<span data-ttu-id="4e20d-110">**疑难解答**</span><span class="sxs-lookup"><span data-stu-id="4e20d-110">**Troubleshooting**</span></span>

<span data-ttu-id="4e20d-111">如果你按照上述说明进行了操作，并且“**电源**”开关灰显或不可见，请在任务栏上的搜索框中，键入 **设备管理器**，然后在结果列表中选择“**设备管理器**”。</span><span class="sxs-lookup"><span data-stu-id="4e20d-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="4e20d-112">在“**电池**”下，右键单击设备的电池，单击“**禁用**”，然后单击“**是**”。</span><span class="sxs-lookup"><span data-stu-id="4e20d-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="4e20d-113">稍等几秒钟，右键单击电池，然后单击“**启用**”。</span><span class="sxs-lookup"><span data-stu-id="4e20d-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="4e20d-114">然后重新启动设备。</span><span class="sxs-lookup"><span data-stu-id="4e20d-114">Then restart your device.</span></span>

<span data-ttu-id="4e20d-115">如果你按照上述说明进行了操作，但电池图标未显示在任务栏上，请在任务栏上的搜索框中键入 **任务管理器**，然后在结果列表中单击“**任务管理器**”。</span><span class="sxs-lookup"><span data-stu-id="4e20d-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="4e20d-116">在“**进程**”选项卡的“**名称**”下，右键单击 **资源管理器**，然后单击“**重新启动**”。</span><span class="sxs-lookup"><span data-stu-id="4e20d-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
