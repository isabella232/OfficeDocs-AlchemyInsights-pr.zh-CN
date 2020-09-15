---
title: 现有监视器疑难解答
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690701"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="8dd51-102">排除现有监视器的故障</span><span class="sxs-lookup"><span data-stu-id="8dd51-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="8dd51-103">请尝试使用以下解决方案对显示器进行故障排除。</span><span class="sxs-lookup"><span data-stu-id="8dd51-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="8dd51-104">**刷新监视器的显示：**</span><span class="sxs-lookup"><span data-stu-id="8dd51-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="8dd51-105">同时按以下键： Windows 键 + Ctrl + Shift + B。这将刷新与您的图形驱动程序的通信。</span><span class="sxs-lookup"><span data-stu-id="8dd51-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="8dd51-106">你的监视器将短暂闪烁并在几秒钟后返回回来。</span><span class="sxs-lookup"><span data-stu-id="8dd51-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="8dd51-107">**监视器硬件故障排除：**</span><span class="sxs-lookup"><span data-stu-id="8dd51-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="8dd51-108">拔下将电脑连接到显示器的电缆，然后重新插回。</span><span class="sxs-lookup"><span data-stu-id="8dd51-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="8dd51-109">断开电脑 (等所有非必要设备，如适配器或停靠) 。</span><span class="sxs-lookup"><span data-stu-id="8dd51-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="8dd51-110">**如果你最近在你的电脑上安装了更新，则可以回滚你的显示驱动程序：**</span><span class="sxs-lookup"><span data-stu-id="8dd51-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="8dd51-111">选择 " **开始**"，键入 " **设备管理器**"，然后从结果中选择 " **设备管理器** "。</span><span class="sxs-lookup"><span data-stu-id="8dd51-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="8dd51-112">展开 " **显示适配器** " 部分，右键单击您的显示适配器，用 and "选择 **属性**"。</span><span class="sxs-lookup"><span data-stu-id="8dd51-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="8dd51-113">导航到 " **驱动程序** " 选项卡，然后选择 " **返回驱动程序**"。</span><span class="sxs-lookup"><span data-stu-id="8dd51-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="8dd51-114">注意：如果此方法不可用或显示为灰色，请从以下选项中选择 " **否** " 以移到下一步。</span><span class="sxs-lookup"><span data-stu-id="8dd51-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="8dd51-115">您可能需要重新启动电脑，这些更改才会生效。</span><span class="sxs-lookup"><span data-stu-id="8dd51-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="8dd51-116">**卸载并重新安装您的显示驱动程序：**</span><span class="sxs-lookup"><span data-stu-id="8dd51-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="8dd51-117">选择 " **开始**"，键入 " **设备管理器**"，然后从结果中选择 " **设备管理器** "。</span><span class="sxs-lookup"><span data-stu-id="8dd51-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="8dd51-118">展开 " **显示适配器** " 部分，右键单击您的显示适配器，用 and "选择 **卸载设备**"。</span><span class="sxs-lookup"><span data-stu-id="8dd51-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="8dd51-119">选择 " **删除此设备的驱动程序软件** " 旁边的框，然后选择 " **卸载**"。</span><span class="sxs-lookup"><span data-stu-id="8dd51-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="8dd51-120">注意：系统可能会要求您在此阶段重新启动计算机。</span><span class="sxs-lookup"><span data-stu-id="8dd51-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="8dd51-121">重新启动之前，请务必记下剩余的说明。</span><span class="sxs-lookup"><span data-stu-id="8dd51-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="8dd51-122">再次打开 "设备管理器"。</span><span class="sxs-lookup"><span data-stu-id="8dd51-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="8dd51-123">展开 " **显示适配器** " 部分，右键单击您的显示适配器，然后选择 " **更新驱动程序**"。</span><span class="sxs-lookup"><span data-stu-id="8dd51-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="8dd51-124">**为更新驱动程序软件选择 "自动搜索**"，然后按照安装说明进行操作。</span><span class="sxs-lookup"><span data-stu-id="8dd51-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>