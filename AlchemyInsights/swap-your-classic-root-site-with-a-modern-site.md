---
title: 将经典根网站替换为新式网站
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
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691169"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>将经典根网站替换为新式网站

如果您的环境是在2019年4月之前设置的，则可以使用 Microsoft PowerShell 将您的根网站更改为新式网站：

- 如果您有一个要用作根网站的不同网站，则可以 [ 将 (交换) 根](https://docs.microsoft.com/sharepoint/modern-root-site) 网站替换为该网站。 
    - 使用 [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) 可在存档原始网站的同时，将网站的位置替换为其他网站。 可用于两个工作组网站 (未连接到组) 和通信网站。 

- 将很快引入其他功能，从而使您能够继续使用网站上的内容，但将现有网站转换为通信网站。 
>[!Important]
>这些功能将逐步推出。 继续检查消息中心是否有更新。 

## <a name="known-issues-with-swapping-sites"></a>交换网站的已知问题

- 在较短的时间内，目标网站可能会返回 "找不到" (HTTP 404) 错误。
- 需要重新爬网内容才能更新搜索索引。 无需手动执行步骤-这将自动完成。
- 依赖于 "静态" 链接 (（如文件同步和 OneNote) 文件）的任何内容都需要手动更正。
- 如果源网站是组织的新闻网站，请更新该 URL。获取所有组织新闻网站的列表。
- 可能需要验证 Project Server 网站，以确保它们仍正确关联。
