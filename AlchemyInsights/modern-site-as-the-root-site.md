---
title: 作为根网站的新式网站
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327592"
---
# <a name="modern-site-as-root-site"></a>作为根网站的新式网站

我们已开始推出一项新功能，将允许你将经典网站根网站 [与新式网站交换](https://docs.microsoft.com/sharepoint/modern-root-site)。 使用 [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) 在存档原始站点时，将站点的位置与另一个站点交换。 适用于未连接到组 (通信网站的工作组) 网站。

**重要** 提示：请勿删除经典根网站以创建新式通信网站。 Microsoft 不支持此功能。 删除根网站会使SharePoint所有用户无法访问您组织的所有网站，直到您在同一 URL 处还原网站或创建新网站。 我们将通过消息中心传达此功能。 你预计功能不久将在租户中打开。

## <a name="known-issues-with-swapping-sites"></a>交换网站的已知问题
- 目标网站可能会在短时间内返回 HTTP 404 (") "找不到"错误。
- 需要重新对内容进行重新绘制以更新搜索索引。 此处无需手动步骤，这将自动完成。
- 任何依赖于"静态"链接 (文件同步和OneNote文件) 需要手动更正。
- Project可能需要验证服务器网站以确保它们仍然正确关联。 
