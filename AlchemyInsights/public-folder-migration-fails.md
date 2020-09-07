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
# <a name="public-folder-migration-fails-at-95"></a>公用文件夹迁移失败，进度为 95%

你可能已启动迁移批处理的完成阶段，但迁移批处理的状态在很长一段时间内持续显示为“**已同步**”。 这是正常的现象。

迁移批处理的状态往往会仍保持在“**已同步**”状态几个小时，然后才会切换到“**正在完成**”。 对于涉及大量目标邮箱的迁移，如果没有任何基础公用文件夹迁移请求失败或被隔离，则保持在已同步状态超过 24 小时的情况是正常的。 请为迁移批处理留出 24-48 小时的时间来完成任务。

对于公用文件夹迁移失败，进度为 95% 且显示 FailedToMailEnablePublicFoldersException 错误的情况：

1. 请在 Exchange 本地服务器上下载和运行 [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF)。

2. 执行脚本建议的纠正措施。

3. 运行 Sync-MailPublicFolders（针对 Exchange 2010）或 Sync-ModernMailPublicFolders（针对 Exchange 2013 及更高版本）。

4. 恢复公用文件夹迁移。
