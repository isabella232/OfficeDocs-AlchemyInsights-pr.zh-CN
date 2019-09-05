---
title: 新式网站作为根网站
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753894"
---
# <a name="modern-site-as-root-site"></a>新式网站作为根网站

我们已经开始推出新功能，使你能够将[经典网站根网站替换为新式网站](https://docs.microsoft.com/sharepoint/modern-root-site)。 使用[SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)可在存档原始网站的同时，将网站的位置替换为其他网站。 可用于两个工作组网站（未连接到组）和通信网站。

>[!Important]
> 请勿删除经典根网站来创建新式通信网站。 Microsoft 不支持这种情况。 删除根网站将使组织中的所有 SharePoint 网站对所有用户不可访问，直到您还原网站或在相同的 URL 上创建新网站。 我们将通过消息中心传达此功能。 你应该会在你的租户中很快启用此功能。

## <a name="known-issues-with-swapping-sites"></a>交换网站的已知问题
- 目标网站可能会在短时间内返回 "未找到" （HTTP 404）错误。
- 需要重新爬网内容才能更新搜索索引。 此处不需要手动步骤，这将自动完成。
- 依赖于 "静态" 链接的任何内容（如文件同步和 OneNote 文件）都需要手动更正。
- 可能需要验证 Project Server 网站，以确保它们仍正确关联。 
