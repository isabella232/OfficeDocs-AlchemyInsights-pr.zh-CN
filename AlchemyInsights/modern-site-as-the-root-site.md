---
title: 新式网站作为根网站
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 6166493f79379f44b1a9bbbaca6becfe624fe912
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057675"
---
# <a name="modern-site-as-root-site"></a>新式网站作为根网站

[目标版本](https://docs.microsoft.com/en-us/office365/admin/manage/release-options-in-office-365?view=o365-worldwide)客户现在可以在其 SharePoint 租户的经典根网站上启用新式通信网站体验。

可以通过运行一个简单的 PowerShell cmdlet 来激活此功能。 在成功执行 PowerShell 命令之后, 根网站将具有新的通信网站主页。 有关 PowerShell cmdlet 和功能要求的详细信息, 请参阅文章[SPOCommSite](https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/Enable-SPOCommSite?view=sharepoint-ps)中提供的。 

默认情况下, 我们会逐步将其关闭, 并在 2019 6 月6日结束时2019在全球范围内提供目标版本的客户, 并在全球范围内推出。 继续使用新式的其他新功能引用[消息中心](https://admin.microsoft.com/AdminPortal/Home#/MessageCenter)。 

**重要说明**: 请勿删除经典根网站来创建新式通信网站。 Microsoft 不支持这种情况。 删除根网站将使组织中的所有 SharePoint 网站对所有用户不可访问, 直到您还原网站或在相同的 URL 上创建新网站。 
 
 