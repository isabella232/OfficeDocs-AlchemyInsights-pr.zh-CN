---
title: 公用文件夹迁移失败，进度为 95%
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: fc8da45d91d5c32be52e48770e469cf25eb068f5
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/26/2020
ms.locfileid: "46903522"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="d3768-102">公用文件夹迁移失败，进度为 95%</span><span class="sxs-lookup"><span data-stu-id="d3768-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="d3768-103">对于公用文件夹迁移失败，进度为 95% 且显示 FailedToMailEnablePublicFoldersException 错误的情况：</span><span class="sxs-lookup"><span data-stu-id="d3768-103">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="d3768-104">请在 Exchange 本地服务器上下载和运行 [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF)。</span><span class="sxs-lookup"><span data-stu-id="d3768-104">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="d3768-105">执行脚本建议的纠正措施。</span><span class="sxs-lookup"><span data-stu-id="d3768-105">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="d3768-106">运行 Sync-MailPublicFolders（针对 Exchange 2010）或 Sync-ModernMailPublicFolders（针对 Exchange 2013 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d3768-106">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="d3768-107">恢复公用文件夹迁移。</span><span class="sxs-lookup"><span data-stu-id="d3768-107">Resume public folder migration.</span></span>
