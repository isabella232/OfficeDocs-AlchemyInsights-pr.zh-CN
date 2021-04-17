---
title: 现有监视器疑难解答
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824569"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="fd367-102">现有监视器疑难解答</span><span class="sxs-lookup"><span data-stu-id="fd367-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="fd367-103">尝试这些解决方案对监视器进行疑难解答。</span><span class="sxs-lookup"><span data-stu-id="fd367-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="fd367-104">**刷新监视器的显示：**</span><span class="sxs-lookup"><span data-stu-id="fd367-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="fd367-105">同时按以下键：Windows 键 + Ctrl + Shift + B。这将刷新与图形驱动程序的通信。</span><span class="sxs-lookup"><span data-stu-id="fd367-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="fd367-106">监视器将暂时闪烁，几秒钟后将返回。</span><span class="sxs-lookup"><span data-stu-id="fd367-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="fd367-107">**监视器硬件疑难解答：**</span><span class="sxs-lookup"><span data-stu-id="fd367-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="fd367-108">拔下电脑与显示器的连接电缆，然后重新插入。</span><span class="sxs-lookup"><span data-stu-id="fd367-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="fd367-109">断开电脑上所有不必要的设备（例如适配器或扩展坞）的连接。</span><span class="sxs-lookup"><span data-stu-id="fd367-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="fd367-110">**如果你最近在你的电脑上安装了更新，你可以回滚显示驱动程序：**</span><span class="sxs-lookup"><span data-stu-id="fd367-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="fd367-111">选择 **"开始**"， **键入设备管理器**，然后 **从结果中选择"设备** 管理器"。</span><span class="sxs-lookup"><span data-stu-id="fd367-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="fd367-112">展开"**显示适配器"** 部分，右键单击显示适配器，然后选择"属性 **"。**</span><span class="sxs-lookup"><span data-stu-id="fd367-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="fd367-113">导航到驱动程序 **选项卡** ，然后选择 **回滚驱动程序**。</span><span class="sxs-lookup"><span data-stu-id="fd367-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="fd367-114">注意：如果不可用或灰显，请从以下选项中选择"否"以移动到下一步。</span><span class="sxs-lookup"><span data-stu-id="fd367-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="fd367-115">你可能需要重新启动电脑，这些更改才能生效。</span><span class="sxs-lookup"><span data-stu-id="fd367-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="fd367-116">**卸载并重新安装显示驱动程序：**</span><span class="sxs-lookup"><span data-stu-id="fd367-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="fd367-117">选择 **"开始**"， **键入设备管理器**，然后 **从结果中选择"设备** 管理器"。</span><span class="sxs-lookup"><span data-stu-id="fd367-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="fd367-118">展开"**显示适配器"** 部分，右键单击显示适配器，然后选择"**卸载设备"。**</span><span class="sxs-lookup"><span data-stu-id="fd367-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="fd367-119">选中"删除此设备的 **驱动程序软件"旁边的框，** 然后选择"卸载 **"。**</span><span class="sxs-lookup"><span data-stu-id="fd367-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="fd367-120">注意：在此阶段，系统可能会要求你重新启动计算机。</span><span class="sxs-lookup"><span data-stu-id="fd367-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="fd367-121">在重新启动之前，请务必记下剩余的说明。</span><span class="sxs-lookup"><span data-stu-id="fd367-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="fd367-122">再次打开设备管理器。</span><span class="sxs-lookup"><span data-stu-id="fd367-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="fd367-123">展开"**显示适配器"** 部分，右键单击显示适配器，然后选择"**更新驱动程序"。**</span><span class="sxs-lookup"><span data-stu-id="fd367-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="fd367-124">选择 **"自动搜索"以更新驱动程序软件，** 然后按照安装说明进行操作。</span><span class="sxs-lookup"><span data-stu-id="fd367-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>