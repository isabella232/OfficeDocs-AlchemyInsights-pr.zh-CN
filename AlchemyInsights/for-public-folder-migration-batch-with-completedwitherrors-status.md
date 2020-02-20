---
title: 对于具有 CompletedWithErrors 状态的公用文件夹迁移批处理
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3532"
ms.openlocfilehash: 739e9d91f90e4c0374814d199e4372eb5625553a
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158588"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="e5504-102">对于具有 CompletedWithErrors 状态的公用文件夹迁移批处理</span><span class="sxs-lookup"><span data-stu-id="e5504-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="e5504-103">使用以下步骤完成批处理，跳过大型/坏项：</span><span class="sxs-lookup"><span data-stu-id="e5504-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="e5504-104">批准迁移批处理上跳过的项目：</span><span class="sxs-lookup"><span data-stu-id="e5504-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="e5504-105">使用以下命令可批准已同步但未完成的迁移请求上跳过的项目：</span><span class="sxs-lookup"><span data-stu-id="e5504-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="e5504-106">迁移批处理和请求应在几分钟后恢复并完成。</span><span class="sxs-lookup"><span data-stu-id="e5504-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

