---
title: 在 Windows 10 中运行 Windows 内存诊断
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: f2b8306d0cd604b144b82275243c5a84580bc609
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720780"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="d6a00-102">在 Windows 10 中运行 Windows 内存诊断</span><span class="sxs-lookup"><span data-stu-id="d6a00-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="d6a00-103">如果电脑上的 Windows 和应用程序崩溃、冻结或操作方式不稳定，则可能是电脑内存 (RAM) 有问题。</span><span class="sxs-lookup"><span data-stu-id="d6a00-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="d6a00-104">可运行 Windows 内存诊断来检查电脑 RAM 的问题。</span><span class="sxs-lookup"><span data-stu-id="d6a00-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="d6a00-105">在任务栏上的搜索框中，键入**内存诊断**，然后选择“**Windows 内存诊断**”。</span><span class="sxs-lookup"><span data-stu-id="d6a00-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="d6a00-106">要运行诊断，需要重启电脑。</span><span class="sxs-lookup"><span data-stu-id="d6a00-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="d6a00-107">可选择立即重启（请先保存你的工作，然后关闭打开的文档和电子邮件），或计划在下次重启电脑时自动运行诊断：</span><span class="sxs-lookup"><span data-stu-id="d6a00-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Windows 内存诊断](media/windows-memory-diagnostic.png)

<span data-ttu-id="d6a00-109">电脑重启时，**Windows 内存诊断工具**将自动运行。</span><span class="sxs-lookup"><span data-stu-id="d6a00-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="d6a00-110">运行诊断时将显示状态和进度，你可以选择通过点击键盘上的 **ESC** 键来取消诊断。</span><span class="sxs-lookup"><span data-stu-id="d6a00-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="d6a00-111">诊断完成后，Windows 将正常启动。</span><span class="sxs-lookup"><span data-stu-id="d6a00-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="d6a00-112">重启后显示桌面时，将立即显示一则通知（任务栏上的**操作中心**图标旁边），指示是否发现了任何内存错误。</span><span class="sxs-lookup"><span data-stu-id="d6a00-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="d6a00-113">例如：</span><span class="sxs-lookup"><span data-stu-id="d6a00-113">For example:</span></span>

<span data-ttu-id="d6a00-114">这是操作中心图标：</span><span class="sxs-lookup"><span data-stu-id="d6a00-114">Here's the Action Center icon:</span></span> ![操作中心图标](media/action-center-icon.png) 

<span data-ttu-id="d6a00-116">和示例通知：</span><span class="sxs-lookup"><span data-stu-id="d6a00-116">And a sample notification:</span></span> ![无内存错误](media/no-memory-errors.png)

<span data-ttu-id="d6a00-118">如果错过了通知，可以选择任务栏上的**操作中心**图标，以显示**操作中心**并查看可滚动的通知列表。</span><span class="sxs-lookup"><span data-stu-id="d6a00-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="d6a00-119">若要查看详细信息，请在任务栏上的搜索框中键入**事件**，然后选择“**事件查看器**”。</span><span class="sxs-lookup"><span data-stu-id="d6a00-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="d6a00-120">在**事件查看器**的左侧窗格中，导航到“**Windows 日志 > 系统**”。</span><span class="sxs-lookup"><span data-stu-id="d6a00-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="d6a00-121">在右侧窗格中，向下搜寻列表的“**源**”列，直至看到带有源值 **MemoryDiagnostics** 的事件。</span><span class="sxs-lookup"><span data-stu-id="d6a00-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="d6a00-122">突出显示每个此类事件，并在列表下方“**常规**”选项卡下的框中查看结果信息。</span><span class="sxs-lookup"><span data-stu-id="d6a00-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
