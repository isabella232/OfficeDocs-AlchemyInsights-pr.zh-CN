---
title: 修复 Windows 10 中的蓝牙问题
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730149"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="23f25-102">修复 Windows 10 中的蓝牙问题</span><span class="sxs-lookup"><span data-stu-id="23f25-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="23f25-103">如果缺少蓝牙图标或蓝牙无法打开或关闭蓝牙，您可能需要运行蓝牙疑难解答。</span><span class="sxs-lookup"><span data-stu-id="23f25-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="23f25-104">[打开 "疑难解答设置](ms-settings:troubleshoot)"，在 "**查找并修复其他问题**" 下单击 "**蓝牙**"，单击 **"运行疑难解答"**。</span><span class="sxs-lookup"><span data-stu-id="23f25-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="23f25-105">如果看不到蓝牙图标，但设备管理器中显示蓝牙：</span><span class="sxs-lookup"><span data-stu-id="23f25-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="23f25-106">在设备管理器中，单击 " **蓝牙**"。</span><span class="sxs-lookup"><span data-stu-id="23f25-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="23f25-107">按住 (或右键单击蓝牙适配器名称) 并单击 " **卸载设备**"。</span><span class="sxs-lookup"><span data-stu-id="23f25-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="23f25-108">关闭 Windows 设备，等待几秒钟，然后将其重新打开。</span><span class="sxs-lookup"><span data-stu-id="23f25-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="23f25-109">Windows 将尝试重新安装驱动程序。</span><span class="sxs-lookup"><span data-stu-id="23f25-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="23f25-110">如果你最近安装了 Windows 10 更新或升级到 Windows 10，你可能需要检查驱动程序更新：</span><span class="sxs-lookup"><span data-stu-id="23f25-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="23f25-111">在 "设备管理器" 中，单击 " **蓝牙**"，然后单击蓝牙适配器名称 (可能包含单词 "收音机" ) 。</span><span class="sxs-lookup"><span data-stu-id="23f25-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="23f25-112">长按 (或右键单击蓝牙适配器) ，然后单击 "自动**更新驱动程序**  >  **搜索" 以更新驱动程序软件**。</span><span class="sxs-lookup"><span data-stu-id="23f25-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="23f25-113">按照步骤操作，然后单击 " **关闭**"。</span><span class="sxs-lookup"><span data-stu-id="23f25-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="23f25-114">如果 Windows 找不到新的蓝牙驱动程序，请访问电脑制造商的网站并从那里下载最新的蓝牙驱动程序。</span><span class="sxs-lookup"><span data-stu-id="23f25-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="23f25-115">下载后，单击 "**更新驱动**程序"  >  **。浏览 "我的电脑" 以驱动程序软件**  >  **浏览**存储驱动程序文件的位置 >**确定 "**  >  **下一步**"，然后按照步骤进行安装。</span><span class="sxs-lookup"><span data-stu-id="23f25-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="23f25-116">安装更新后的驱动程序后，重新启动计算机，然后检查是否修复了连接问题。</span><span class="sxs-lookup"><span data-stu-id="23f25-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="23f25-117">有关如何解决蓝牙问题的更多详细信息，请参阅完整文章， [修复 Windows 10 中的蓝牙问题](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)。</span><span class="sxs-lookup"><span data-stu-id="23f25-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
