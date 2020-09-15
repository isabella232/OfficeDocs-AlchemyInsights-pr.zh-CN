---
title: 内容搜索无结果
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
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680637"
---
# <a name="no-results-from-content-searchexports"></a>内容搜索/导出没有结果

不返回任何数据的内容搜索/导出的问题可能是由于特定管理员设置的某些合规性安全筛选器而不是将其与所有管理员通信。

若要解决此问题，请检查是否存在可能导致此问题的合规性安全筛选器：
1. 连接到安全与合规中心 Powershell
2. 运行以下 commandlet：
<br>$org = "yourdomain.com"
<br>New-compliancesecurityfilter-组织 $org