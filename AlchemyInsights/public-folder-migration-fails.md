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
ms.openlocfilehash: c1c4210baf93f0071a12f1902fb5f6fbf7bd0716
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341382"
---
# <a name="public-folder-migration-fails-at-95"></a><span data-ttu-id="c4bfe-102">公用文件夹迁移失败，进度为 95%</span><span class="sxs-lookup"><span data-stu-id="c4bfe-102">Public folder migration fails at 95%</span></span>

<span data-ttu-id="c4bfe-103">你可能已启动迁移批处理的完成阶段，但迁移批处理的状态在很长一段时间内持续显示为“**已同步**”。</span><span class="sxs-lookup"><span data-stu-id="c4bfe-103">You might have initiated completion of a migration batch, and the status of the migration batch continues showing **Synced** for a very long time.</span></span> <span data-ttu-id="c4bfe-104">这是正常的现象。</span><span class="sxs-lookup"><span data-stu-id="c4bfe-104">This is expected behavior.</span></span>

<span data-ttu-id="c4bfe-105">迁移批处理的状态往往会仍保持在“**已同步**”状态几个小时，然后才会切换到“**正在完成**”。</span><span class="sxs-lookup"><span data-stu-id="c4bfe-105">It's common for the status of a migration batch to remain on **Synced** for a few hours before it switches to **Completing**.</span></span> <span data-ttu-id="c4bfe-106">对于涉及大量目标邮箱的迁移，如果没有任何基础公用文件夹迁移请求失败或被隔离，则保持在已同步状态超过 24 小时的情况是正常的。</span><span class="sxs-lookup"><span data-stu-id="c4bfe-106">For migrations involving a large number of target mailboxes, it's normal to see the status remain in the synced state for more than 24 hours, provided none of the underlying public folder migration requests have failed or were quarantined.</span></span> <span data-ttu-id="c4bfe-107">请为迁移批处理留出 24-48 小时的时间来完成任务。</span><span class="sxs-lookup"><span data-stu-id="c4bfe-107">Please allow 24-48 hours for the migration batch to complete the tasks.</span></span>

<span data-ttu-id="c4bfe-108">对于公用文件夹迁移失败，进度为 95% 且显示 FailedToMailEnablePublicFoldersException 错误的情况：</span><span class="sxs-lookup"><span data-stu-id="c4bfe-108">For public folder migrations failing at 95%, with error FailedToMailEnablePublicFoldersException:</span></span>

1. <span data-ttu-id="c4bfe-109">请在 Exchange 本地服务器上下载和运行 [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF)。</span><span class="sxs-lookup"><span data-stu-id="c4bfe-109">Download and run the [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) script at your Exchange On-Premises server.</span></span>

2. <span data-ttu-id="c4bfe-110">执行脚本建议的纠正措施。</span><span class="sxs-lookup"><span data-stu-id="c4bfe-110">Perform the corrective actions suggested by the script.</span></span>

3. <span data-ttu-id="c4bfe-111">运行 Sync-MailPublicFolders（针对 Exchange 2010）或 Sync-ModernMailPublicFolders（针对 Exchange 2013 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="c4bfe-111">Run the Sync-MailPublicFolders (for Exchange 2010) or Sync-ModernMailPublicFolders (for Exchange 2013 and later).</span></span>

4. <span data-ttu-id="c4bfe-112">恢复公用文件夹迁移。</span><span class="sxs-lookup"><span data-stu-id="c4bfe-112">Resume public folder migration.</span></span>
