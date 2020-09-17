---
title: 双击 Office 文件无法打开它
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
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812069"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="2acc4-102">双击 Office 文件无法打开它</span><span class="sxs-lookup"><span data-stu-id="2acc4-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="2acc4-103">双击 Office 文件后，您可能会看到该程序打开，但文件本身并不打开。</span><span class="sxs-lookup"><span data-stu-id="2acc4-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="2acc4-104">或者，您可能会收到错误： "将命令发送到程序时出现问题。"</span><span class="sxs-lookup"><span data-stu-id="2acc4-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="2acc4-105">导致此问题的原因有很多，但两个最常见的解决方案是：</span><span class="sxs-lookup"><span data-stu-id="2acc4-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="2acc4-106">在 Excel 中，确保未选中 DDE 选项。</span><span class="sxs-lookup"><span data-stu-id="2acc4-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="2acc4-107">可以通过创建新的工作簿，然后选择 " **文件 > 选项" > 高级**"来找到该选项。</span><span class="sxs-lookup"><span data-stu-id="2acc4-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="2acc4-108">在 " **常规** " 部分中，取消选中 " \*\*忽略使用动态数据交换的其他应用程序 (DDE) \*\*"。</span><span class="sxs-lookup"><span data-stu-id="2acc4-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="2acc4-109">运行联机修复以还原默认设置。</span><span class="sxs-lookup"><span data-stu-id="2acc4-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="2acc4-110">单击 Windows "开始" 按钮，然后搜索 "控制面板"。</span><span class="sxs-lookup"><span data-stu-id="2acc4-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="2acc4-111">打开 " **控制面板**"，然后转到 " **程序" > "程序和功能**"。</span><span class="sxs-lookup"><span data-stu-id="2acc4-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="2acc4-112">然后右键单击 " **Microsoft Office [Version]** "，然后选择 " **更改 > 联机修复**"。</span><span class="sxs-lookup"><span data-stu-id="2acc4-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="2acc4-113">如果这两种解决方案都不起作用，则可以在支持文章中找到更完整的解决方案列表， [双击 Office 文件将无法打开它](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)。</span><span class="sxs-lookup"><span data-stu-id="2acc4-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
