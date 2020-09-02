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
ms.openlocfilehash: fc8da45d91d5c32be52e48770e469cf25eb068f5
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/26/2020
ms.locfileid: "46903522"
---
# <a name="public-folder-migration-fails-at-95"></a>公用文件夹迁移失败，进度为 95%

对于公用文件夹迁移失败，进度为 95% 且显示 FailedToMailEnablePublicFoldersException 错误的情况：

1. 请在 Exchange 本地服务器上下载和运行 [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF)。

2. 执行脚本建议的纠正措施。

3. 运行 Sync-MailPublicFolders（针对 Exchange 2010）或 Sync-ModernMailPublicFolders（针对 Exchange 2013 及更高版本）。

4. 恢复公用文件夹迁移。
