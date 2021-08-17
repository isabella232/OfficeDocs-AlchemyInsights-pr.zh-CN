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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057992"
---
# <a name="no-results-from-content-searchexports"></a>没有来自内容搜索/导出的结果

内容搜索/导出未返回任何数据的问题可能是由于特定管理员设置的特定合规性安全筛选器，未将它传达到所有管理员。

若要解决此问题，请检查是否有可能导致此情况出现的任何合规性安全筛选器：
1. 连接安全与合规中心 Powershell
2. 运行以下命令let：
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org