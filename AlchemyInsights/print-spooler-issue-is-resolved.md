---
title: 打印后台处理程序问题已解决
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 53b1c9a8efa3cc978af8b602c8ed90430042186a
ms.sourcegitcommit: 4265a9e79db6c2a396aa80ec0ebd467bbaadf366
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45083924"
---
# <a name="print-spooler-issue-is-resolved"></a><span data-ttu-id="03c8a-102">打印后台处理程序问题已解决</span><span class="sxs-lookup"><span data-stu-id="03c8a-102">Print spooler issue is resolved</span></span>

<span data-ttu-id="03c8a-103">如果你的设备已使用 Windows 10 **操作系统内部版本 19041.329** 进行更新，你可能已观察到某些打印机无法进行打印的问题。</span><span class="sxs-lookup"><span data-stu-id="03c8a-103">If your device was updated with Windows 10  **OS Build 19041.329**, you might have observed an issue where certain printers fail to print.</span></span> <span data-ttu-id="03c8a-104">打印后台处理程序可能会在尝试打印时抛出错误或意外关闭，并且受影响的打印机没有输出。</span><span class="sxs-lookup"><span data-stu-id="03c8a-104">The print spooler might throw an error or close unexpectedly when attempting to print, and no output comes from the affected printer.</span></span> <span data-ttu-id="03c8a-105">该问题已在操作系统内部版本 **19041.331** 中得到解决，[KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523)。</span><span class="sxs-lookup"><span data-stu-id="03c8a-105">This issue is resolved in OS Build  **19041.331**, [KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523).</span></span>  

<span data-ttu-id="03c8a-106">**持续调查**</span><span class="sxs-lookup"><span data-stu-id="03c8a-106">**Ongoing investigation**</span></span>

<span data-ttu-id="03c8a-107">本地安全机构子系统服务 (LSASS) 文件 (**Isass.exe**) 在某些设备上可能无法使用，显示错误消息“关键系统进程 C:\WINDOWS\system32\Isass.exe 失败，状态代码是 c0000008。</span><span class="sxs-lookup"><span data-stu-id="03c8a-107">The Local Security Authority Subsystem Service (LSASS) file (**Isass.exe**) might fail on some devices with the error message, "A critical system process, C:\WINDOWS\system32\Isass.exe, failed with status code c0000008.</span></span> <span data-ttu-id="03c8a-108">现在必须重新启动计算机。”</span><span class="sxs-lookup"><span data-stu-id="03c8a-108">The machine must now be restarted".</span></span>  <span data-ttu-id="03c8a-109">**Microsoft 正在努力解决问题，并将在即将发布的版本中提供更新。**</span><span class="sxs-lookup"><span data-stu-id="03c8a-109">**Microsoft is working on a resolution and will provide an update in an upcoming release.**</span></span>

<span data-ttu-id="03c8a-110">有关详细信息，请参阅 [Windows 10 版本 2004 中的已知问题](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)。</span><span class="sxs-lookup"><span data-stu-id="03c8a-110">For more information, please check out  [Windows 10 Version 2004 known issues](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc).</span></span>