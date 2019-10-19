---
title: 将经典根网站替换为新式网站
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: bd477d90ab7e6737aafffc57d931aad2bd0351e8
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36749250"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>将经典根网站替换为新式网站

如果您的环境是在2019年4月之前设置的，则可以使用 Microsoft PowerShell 将您的根网站更改为新式网站：

- 如果您有一个要用作根网站的不同网站，则可以将[根网站替换（交换）](https://docs.microsoft.com/sharepoint/modern-root-site)到根网站。 
    - 使用[SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)可在存档原始网站的同时，将网站的位置替换为其他网站。 可用于两个工作组网站（未连接到组）和通信网站。 

- 将很快引入其他功能，从而使您能够继续使用网站上的内容，但将现有网站转换为通信网站。 
>[!Important]
>这些功能将逐步推出。 继续检查 Office 365 消息中心是否有更新。 

## <a name="known-issues-with-swapping-sites"></a>交换网站的已知问题

- 目标网站可能会在短时间内返回 "未找到" （HTTP 404）错误。
- 需要重新爬网内容才能更新搜索索引。 无需手动执行步骤-这将自动完成。
- 依赖于 "静态" 链接的任何内容（如文件同步和 OneNote 文件）都需要手动更正。
- 如果源网站是组织的新闻网站，请更新该 URL。获取所有组织新闻网站的列表。
- 可能需要验证 Project Server 网站，以确保它们仍正确关联。





