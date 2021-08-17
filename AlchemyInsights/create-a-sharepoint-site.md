---
title: 创建 SharePoint 网站
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: bf9380727fff415357884a5122e633f2254337d3db50e2b8656d94938f76d394
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54080880"
---
# <a name="create-a-sharepoint-site"></a>创建 SharePoint 网站

从管理中心[的活动站点](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true)创建SharePoint管理网站。 有关详细信息，请参阅管理[新网站管理SharePoint中的网站](https://docs.microsoft.com/sharepoint/manage-site-creation)。 

## <a name="tips"></a>使用技巧：

- 您不能 **使用** 现有网站的相同 URL 创建网站。 如果已删除网站并且希望重新使用该 URL，则已删除的网站可能仍存在于"已删除网站 ["下](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)。 网站将需要永久删除，以重新使用该 URL。 若要使用 Powershell 完全删除网站，请参阅 [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet 示例。
- 某些用户可能无法创建网站。 [请参阅在 SharePoint Online 中管理网站创建](https://docs.microsoft.com/sharepoint/manage-site-creation)。
- 网站可能卡在"创建 **时间超过** 预期"。 如果自你第一次看到此问题以来超过 24 小时，请记录支持票证。 在许多情况下，我们已经在研究解决方案。 请给我们至少 24 小时才能完成解决方案。
