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
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068154"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>对于具有 CompletedWithErrors 状态的公用文件夹迁移批处理

使用以下步骤完成批处理，跳过大/坏项目： 
1. 批准迁移批处理中跳过的项目：

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. 使用以下命令批准"已同步"但未完成的迁移请求上跳过的项目：

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. 迁移批处理和请求应在几分钟后恢复并完成。

