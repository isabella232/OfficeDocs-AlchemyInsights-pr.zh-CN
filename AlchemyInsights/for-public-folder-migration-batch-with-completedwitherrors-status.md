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
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>对于具有 CompletedWithErrors 状态的公用文件夹迁移批处理

使用以下步骤完成批处理，跳过大型/坏项： 
1. 批准迁移批处理上跳过的项目：

    New-migrationbatch \<batchname>-ApproveSkippedItems 
2. 使用以下命令可批准已同步但未完成的迁移请求上跳过的项目：

    $pf = Remove-publicfoldermailboxmigrationrequest |Get-publicfoldermailboxmigrationrequeststatistics-IncludeReport;ForEach （$i $pf） {if （$i LargeItemsEncountered-gt 0-或 $i BadItemsEncountered-gt 0） {Remove-publicfoldermailboxmigrationrequest $i IdentifyingGuid-SkippedItemApprovalTime $ （[DateTime]：： UtcNow）}}
3. 迁移批处理和请求应在几分钟后恢复并完成。

