---
title: 导入前修复 .pst 文件
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 1ed37192a6b054b745fd48fbc01a6b00fa7074ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799086"
---
# <a name="repair-pst-file-before-importing"></a><span data-ttu-id="5378b-102">导入前修复 .pst 文件</span><span class="sxs-lookup"><span data-stu-id="5378b-102">Repair .pst file before importing</span></span>

<span data-ttu-id="5378b-103">在 Outlook 中导入 .pst 文件之前，请先通过修复文件验证文件是否已损坏：</span><span class="sxs-lookup"><span data-stu-id="5378b-103">Before you import a .pst file in Outlook, verify the file is not corrupted by repairing the file:</span></span>

1. <span data-ttu-id="5378b-104">退出 Outlook。</span><span class="sxs-lookup"><span data-stu-id="5378b-104">Exit Outlook.</span></span>

2. <span data-ttu-id="5378b-105">`Scanpst.exe`在 Office 程序文件夹中查找和运行 (C:\Program 文件 (x86) \Microsoft Office\root\Office \<Version\> 或 C:\Program Files\Microsoft Office\root\Office \<Version\>) 。</span><span class="sxs-lookup"><span data-stu-id="5378b-105">Find and run `Scanpst.exe` in your Office program folder (C:\Program Files (x86)\Microsoft Office\root\Office\<Version\> or C:\Program Files\Microsoft Office\root\Office\<Version\>).</span></span>

3. <span data-ttu-id="5378b-106">在 **Microsoft Outlook 收件箱修复工具**中，单击 " **浏览** " 查找 .pst 文件 (例如，在 C:\Users \\<username \> \AppData\Local\Microsoft\Outlook) 。</span><span class="sxs-lookup"><span data-stu-id="5378b-106">In the **Microsoft Outlook Inbox Repair tool**, click **Browse** to find the .pst file (for example, in C:\Users\\<username\>\AppData\Local\Microsoft\Outlook).</span></span> <span data-ttu-id="5378b-107">选择 .pst 文件，然后单击 " **打开**"。</span><span class="sxs-lookup"><span data-stu-id="5378b-107">Select the .pst file and then click **Open**.</span></span>

4. <span data-ttu-id="5378b-108">单击 " **启动** " 开始扫描。</span><span class="sxs-lookup"><span data-stu-id="5378b-108">Click **Start** to begin the scan.</span></span>

5. <span data-ttu-id="5378b-109">如果在文件中发现错误，请单击 " **修复**"，然后在修复完成后单击 **"确定"** 。</span><span class="sxs-lookup"><span data-stu-id="5378b-109">If errors are found in the file, click **Repair**, and then click **OK** when the repair is complete.</span></span>

6. <span data-ttu-id="5378b-110">尝试重新导入 Outlook 中的 .pst 文件。</span><span class="sxs-lookup"><span data-stu-id="5378b-110">Try to import the .pst file in Outlook again.</span></span>

<span data-ttu-id="5378b-111">有关详细信息，请参阅 [修复 outlook 数据文件](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) 和 [修复导入 Outlook .pst 文件中的问题](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)。</span><span class="sxs-lookup"><span data-stu-id="5378b-111">For more information, see [Repair Outlook data files](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) and [Fix problems importing an Outlook .pst file](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>
