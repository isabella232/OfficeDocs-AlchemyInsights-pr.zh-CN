---
title: 对于具有 CompletedWithErrors 状态的公用文件夹迁移批处理
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
- "3500007"
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744103"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="a97b0-102">对于具有 CompletedWithErrors 状态的公用文件夹迁移批处理</span><span class="sxs-lookup"><span data-stu-id="a97b0-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="a97b0-103">使用以下步骤完成批处理，跳过大型/坏项：</span><span class="sxs-lookup"><span data-stu-id="a97b0-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="a97b0-104">批准迁移批处理上跳过的项目：</span><span class="sxs-lookup"><span data-stu-id="a97b0-104">Approve the skipped items on migration batch:</span></span>

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. <span data-ttu-id="a97b0-105">使用以下命令可批准已同步但未完成的迁移请求上跳过的项目：</span><span class="sxs-lookup"><span data-stu-id="a97b0-105">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. <span data-ttu-id="a97b0-106">迁移批处理和请求应在几分钟后恢复并完成。</span><span class="sxs-lookup"><span data-stu-id="a97b0-106">The migration batch and requests should resume and complete in a few minutes.</span></span>

