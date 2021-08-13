---
title: 永久删除 SharePoint 中的站点
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: f461963c4a5719957258349d667731231023721ab3ee4641538c94371bf3f56d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944301"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>永久删除 SharePoint 中的站点

如要重新使用已删除站点的 URL（来重新创建站点），或永久删除不再使用的站点，可使用新版 SharePoint 管理中心中的“**永久删除**”。  

1. 转到[删除新版 SharePoint 管理中心的站点页面](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true)，然后使用在组织中具有管理员权限的帐户进行登录。 

2. 在左栏中，选择一个站点。 

3. 单击 **永久删除**。 

**注意**：连接到组的站点无法永久从新版 SharePoint 管理中心中删除。 系统将替代使用 [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite)。  

有关详细信息，请参阅[永久删除站点](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site)。 
