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
ms.openlocfilehash: 9f2c0273762f1a4a2b905487f461dc1d05db9209
ms.sourcegitcommit: 8f97342d8b46ab05f1e89018473caad9d35431df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/19/2019
ms.locfileid: "35800202"
---
# <a name="no-results-from-content-searchexports"></a>内容搜索/导出没有结果

不返回任何数据的内容搜索/导出的问题可能是由于特定管理员设置的某些合规性安全筛选器而不是将其与所有管理员通信。

若要解决此问题, 请检查是否存在可能导致此问题的合规性安全筛选器:
1. 连接到安全与合规中心 Powershell
2. 运行以下 commandlet:
<br>$org = "yourdomain.com"
<br>New-compliancesecurityfilter-组织 $org