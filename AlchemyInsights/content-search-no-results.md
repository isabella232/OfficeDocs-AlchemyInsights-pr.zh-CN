---
title: 内容搜索无结果
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000661"
- "2527"
ms.openlocfilehash: 09cdbc3cb0465e0e0bc08872c49e283081ad3e92
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516769"
---
# <a name="no-results-from-content-searchexports"></a>内容搜索/导出没有结果

不返回任何数据的内容搜索/导出的问题可能是由于特定管理员设置的某些合规性安全筛选器而不是将其与所有管理员通信。

若要解决此问题, 请检查是否存在可能导致此问题的合规性安全筛选器:
1. 连接到安全与合规中心 Powershell
2. 运行以下 commandlet:
<br>$org = "yourdomain.com"
<br>New-compliancesecurityfilter-组织 $org