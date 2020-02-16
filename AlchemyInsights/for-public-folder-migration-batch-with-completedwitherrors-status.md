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
ms.openlocfilehash: 4243cdf0170fed1eadac6560d2a04e1a861c63e5
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/15/2020
ms.locfileid: "42043569"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a><span data-ttu-id="dbf3d-102">对于具有 CompletedWithErrors 状态的公用文件夹迁移批处理</span><span class="sxs-lookup"><span data-stu-id="dbf3d-102">For Public folder migration batch with CompletedWithErrors status</span></span>

<span data-ttu-id="dbf3d-103">使用以下步骤完成批处理，跳过大型/坏项：</span><span class="sxs-lookup"><span data-stu-id="dbf3d-103">Use the following steps to complete the batch, skipping the large/bad items:</span></span> 
1. <span data-ttu-id="dbf3d-104">批准迁移批处理上跳过的项目：</span><span class="sxs-lookup"><span data-stu-id="dbf3d-104">Approve the skipped items on migration batch:</span></span>

    <span data-ttu-id="dbf3d-105">New-migrationbatch \<batchname>-ApproveSkippedItems</span><span class="sxs-lookup"><span data-stu-id="dbf3d-105">Set-MigrationBatch \<batchname> -ApproveSkippedItems</span></span> 
2. <span data-ttu-id="dbf3d-106">使用以下命令可批准已同步但未完成的迁移请求上跳过的项目：</span><span class="sxs-lookup"><span data-stu-id="dbf3d-106">Use the following command to approve the skipped items on migration requests that are “Synced” but not completed:</span></span>

    <span data-ttu-id="dbf3d-107">$pf = Remove-publicfoldermailboxmigrationrequest |Get-publicfoldermailboxmigrationrequeststatistics-IncludeReport;ForEach （$i $pf） {if （$i LargeItemsEncountered-gt 0-或 $i BadItemsEncountered-gt 0） {Remove-publicfoldermailboxmigrationrequest $i IdentifyingGuid-SkippedItemApprovalTime $ （[DateTime]：： UtcNow）}}</span><span class="sxs-lookup"><span data-stu-id="dbf3d-107">$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}</span></span>
3. <span data-ttu-id="dbf3d-108">迁移批处理和请求应在几分钟后恢复并完成。</span><span class="sxs-lookup"><span data-stu-id="dbf3d-108">The migration batch and requests should resume and complete in a few minutes.</span></span>

