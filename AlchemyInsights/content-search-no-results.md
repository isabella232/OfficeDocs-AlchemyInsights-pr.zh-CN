---
title: 内容搜索无结果
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816838"
---
# <a name="no-results-from-content-searchexports"></a>没有来自内容搜索/导出的结果

内容搜索/导出未返回任何数据的问题可能是由于特定管理员设置的特定合规性安全筛选器，未将它传达到所有管理员。

若要解决此问题，请检查是否有可能导致此情况出现的任何合规性安全筛选器：
1. 连接到安全与合规中心 Powershell
2. 运行以下命令let：
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org