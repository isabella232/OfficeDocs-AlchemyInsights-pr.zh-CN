---
title: 在 Windows 10 中释放驱动器空间
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505346"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="b298e-102">在 Windows 10 中释放驱动器空间</span><span class="sxs-lookup"><span data-stu-id="b298e-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="b298e-103">以下是在 Windows 中释放驱动器空间的两个选项：</span><span class="sxs-lookup"><span data-stu-id="b298e-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="b298e-104">在 Windows 10 中释放驱动器空间。</span><span class="sxs-lookup"><span data-stu-id="b298e-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="b298e-105">通过外部存储设备为 Windows 10 更新释放空间。</span><span class="sxs-lookup"><span data-stu-id="b298e-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="b298e-106">如果使用“磁盘清理”后，磁盘空间仍然不足，则你的 Temp 文件夹可能很快就会被 Microsoft Store 使用的应用程序 (.appx) 文件填满。</span><span class="sxs-lookup"><span data-stu-id="b298e-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="b298e-107">若要修复此问题，请重置 Microsoft Store，清除 Microsoft Store 缓存，然后运行 Windows Update 故障排除程序。</span><span class="sxs-lookup"><span data-stu-id="b298e-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="b298e-108">在继续执行这些步骤之前，请确保 Microsoft Store 已关闭。</span><span class="sxs-lookup"><span data-stu-id="b298e-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="b298e-109">**步骤 1：重置 Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="b298e-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="b298e-110">**注意** 这将永久删除设备上的应用数据，包括首选项和登录详细信息。</span><span class="sxs-lookup"><span data-stu-id="b298e-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="b298e-111">选择“**开始**” > “**设置**” > “**应用**” > “**应用和功能**”。</span><span class="sxs-lookup"><span data-stu-id="b298e-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="b298e-112">在应用列表中，找到并选择“Microsoft Store”。</span><span class="sxs-lookup"><span data-stu-id="b298e-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="b298e-113">选择“**高级选项**”。</span><span class="sxs-lookup"><span data-stu-id="b298e-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="b298e-114">向下滚动并选择“**重置**”，然后选择“**确认重置**”。</span><span class="sxs-lookup"><span data-stu-id="b298e-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="b298e-115">**步骤 2：清除 Microsoft Store 缓存**</span><span class="sxs-lookup"><span data-stu-id="b298e-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="b298e-116">按 Windows 徽标键 + R 以打开“运行”对话框。</span><span class="sxs-lookup"><span data-stu-id="b298e-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="b298e-117">键入 wsreset.exe，然后选择“**确定**”。</span><span class="sxs-lookup"><span data-stu-id="b298e-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="b298e-118">此时会打开一个空白的命令提示符窗口。</span><span class="sxs-lookup"><span data-stu-id="b298e-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="b298e-119">约 10 秒钟后，窗口将关闭并自动打开 Microsoft Store。</span><span class="sxs-lookup"><span data-stu-id="b298e-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="b298e-120">**步骤 3：重置 Windows 更新**</span><span class="sxs-lookup"><span data-stu-id="b298e-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="b298e-121">选择“**开始**” > “**设置**” > “**更新和安全**” > “**故障排除**”。</span><span class="sxs-lookup"><span data-stu-id="b298e-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="b298e-122">向下滚动并从列表中选择“**Windows 更新**”，然后选择“**运行故障排除程序**”。</span><span class="sxs-lookup"><span data-stu-id="b298e-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="b298e-123">重新启动计算机，检查是否仍遇到此问题。</span><span class="sxs-lookup"><span data-stu-id="b298e-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

