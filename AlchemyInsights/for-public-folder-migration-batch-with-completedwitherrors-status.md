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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>对于具有 CompletedWithErrors 状态的公用文件夹迁移批处理

使用以下步骤完成批处理，跳过大型/坏项： 
1. 批准迁移批处理上跳过的项目：

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. 使用以下命令可批准已同步但未完成的迁移请求上跳过的项目：

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. 迁移批处理和请求应在几分钟后恢复并完成。

