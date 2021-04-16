---
title: 双击 Office 文件无法打开它
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
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814795"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="5296c-102">双击 Office 文件无法打开它</span><span class="sxs-lookup"><span data-stu-id="5296c-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="5296c-103">双击 Office 文件后，你可能会看到程序已打开，但文件本身未打开。</span><span class="sxs-lookup"><span data-stu-id="5296c-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="5296c-104">或者，你可能会收到错误："将命令发送到程序时出现问题。"</span><span class="sxs-lookup"><span data-stu-id="5296c-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="5296c-105">出现此现象的原因有很多，但两种最常见的解决方案是：</span><span class="sxs-lookup"><span data-stu-id="5296c-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="5296c-106">在 Excel 中，确保未选中 DDE 选项。</span><span class="sxs-lookup"><span data-stu-id="5296c-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="5296c-107">可通过创建新工作簿，然后选择"文件""选项">"高级"> **找到该选项**。</span><span class="sxs-lookup"><span data-stu-id="5296c-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="5296c-108">在"**常规"** 部分，取消选中"忽略使用动态数据交换的其他应用程序 **(DDE) "。**</span><span class="sxs-lookup"><span data-stu-id="5296c-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="5296c-109">运行联机修复以还原默认设置。</span><span class="sxs-lookup"><span data-stu-id="5296c-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="5296c-110">单击 Windows"开始"按钮并搜索"控制面板"。</span><span class="sxs-lookup"><span data-stu-id="5296c-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="5296c-111">打开 **"控制面板"，** 然后转到"**程序和>程序"。**</span><span class="sxs-lookup"><span data-stu-id="5296c-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="5296c-112">然后右键单击"Microsoft Office **[版本]"，** 然后选择"更改>**联机修复"。**</span><span class="sxs-lookup"><span data-stu-id="5296c-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="5296c-113">如果这两个解决方案都不起作用，可以在支持文章中找到更完整的解决方案列表：双击 Office 文件无法 [打开它](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)。</span><span class="sxs-lookup"><span data-stu-id="5296c-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
