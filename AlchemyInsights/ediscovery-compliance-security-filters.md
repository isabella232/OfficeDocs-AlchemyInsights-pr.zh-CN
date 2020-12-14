---
title: 内容搜索/导出期间未返回任何结果
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/14/2020
ms.locfileid: "49666638"
---
# <a name="no-results-returned-during-content-searchexport"></a>内容搜索/导出期间未返回任何结果

如果遇到以下电子数据展示方案的问题：

- 内容搜索/导出不会返回任何数据或意外数据
- 电子数据展示搜索或导出失败

这可能是由特定管理员设置且未传达给所有管理员的某些合规性安全筛选器导致的。

若要解决此问题，请检查是否有可能导致这些问题的合规性安全筛选器：

1. 连接到安全与合规中心 Powershell
2. 运行以下命令let：

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

有关合规性安全筛选器的其他信息，请参阅 [内容搜索的权限筛选](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
