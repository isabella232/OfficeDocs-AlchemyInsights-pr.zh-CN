---
title: 对于具有 CompletedWithErrors 状态的公用文件夹迁移批处理
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
- "3500007"
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812454"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="ad1b3-102">对于具有 CompletedWithErrors 状态的公用文件夹迁移批处理</span><span class="sxs-lookup"><span data-stu-id="ad1b3-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="ad1b3-103">使用以下步骤完成批处理，跳过大/坏项目：</span><span class="sxs-lookup"><span data-stu-id="ad1b3-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="ad1b3-104">批准迁移批处理中跳过的项目：</span><span class="sxs-lookup"><span data-stu-id="ad1b3-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="ad1b3-105">使用以下命令批准"已同步"但未完成的迁移请求上跳过的项目：</span><span class="sxs-lookup"><span data-stu-id="ad1b3-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="ad1b3-106">迁移批处理和请求应在几分钟后恢复并完成。</span><span class="sxs-lookup"><span data-stu-id="ad1b3-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

