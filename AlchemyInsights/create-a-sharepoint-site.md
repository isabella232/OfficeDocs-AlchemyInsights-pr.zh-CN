---
title: 创建 SharePoint 网站
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: ba682f3c2b2600031f6856621691b1e0fba64113
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786555"
---
# <a name="create-a-sharepoint-site"></a>创建 SharePoint 网站

在 SharePoint 管理中心中创建或管理 [活动网站](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) 中的网站。 有关详细信息，请参阅在 [新 SharePoint 管理中心中管理网站](https://docs.microsoft.com/sharepoint/manage-site-creation)。 

## <a name="tips"></a>几点

- 您 **无法** 使用与现有网站相同的 URL 创建网站。 如果您删除了某个网站，并且希望重新使用该 URL，则可能是已删除的网站仍存在于 " [已删除的网站](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)" 下。 需要永久删除网站以重新使用 URL。 若要使用 Powershell 完全删除站点，请参阅 [remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet 示例。
- 某些用户可能不能创建网站。 [请参阅在 SharePoint Online 中管理网站创建](https://docs.microsoft.com/sharepoint/manage-site-creation)。
- 在 **创建** 比预期更长的时间，网站可能会变得被卡住。 如果在你首次看到此问题后过去已经超过24小时，请记录一个支持票证。 在许多情况下，我们已经在研究解决方案。 请至少为我们提供24小时的时间来完成解决方案。
