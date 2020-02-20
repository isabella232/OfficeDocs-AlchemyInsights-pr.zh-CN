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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>对于具有 CompletedWithErrors 状态的公用文件夹迁移批处理

使用以下步骤完成批处理，跳过大型/坏项： 
1. 批准迁移批处理上跳过的项目：

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. 使用以下命令可批准已同步但未完成的迁移请求上跳过的项目：

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. 迁移批处理和请求应在几分钟后恢复并完成。

