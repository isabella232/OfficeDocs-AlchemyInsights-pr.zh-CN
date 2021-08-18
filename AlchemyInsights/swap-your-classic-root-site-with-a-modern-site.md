---
title: 将经典根网站与新式网站交换
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316130"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>将经典根网站与新式网站交换

如果环境是在 2019 年 4 月之前设置的，可以使用 Microsoft PowerShell 将根网站更改为新式网站：

- 如果您有另一个要用作根网站的网站，可以将 ([ 替换) 替换为](https://docs.microsoft.com/sharepoint/modern-root-site) 根网站。 
    - 使用 [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) 在存档原始站点时，将站点的位置与另一个站点交换。 适用于未连接到组 (通信网站的工作组) 网站。 

- 即将引入其他功能，允许您继续使用网站上的内容，但会将现有网站转换为通信网站。 

**重要** 提示：这些功能将逐步推出。 继续检查消息中心的更新。 

## <a name="known-issues-with-swapping-sites"></a>交换网站的已知问题

- 目标网站可能会在短时间内返回 HTTP 404 (") "找不到"错误。
- 需要重新对内容进行重新绘制以更新搜索索引。 无需手动步骤 - 这将自动完成。
- 任何依赖于"静态"链接 (文件同步和OneNote文件) 需要手动更正。
- 如果源网站是组织新闻网站，请更新 URL。 获取所有组织新闻网站的列表。
- Project可能需要验证服务器网站以确保它们仍然正确关联。
