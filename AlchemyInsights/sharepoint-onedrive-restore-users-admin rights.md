---
title: 对 OneDrive for Business 网站的 "拒绝访问" 消息进行故障排除
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d47ce80bdd07a25d9724057edf0289808a00a3db
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232507"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>对 OneDrive for Business 网站的 "拒绝访问" 消息进行故障排除

在使用相同的用户主体名称 (UPN) 对用户进行删除和重新创建时, 通常会出现此问题。 使用不同的 PUID (Passport 唯一 ID) 值创建新帐户。 当用户尝试访问网站集或其 OneDrive 时, 用户的 PUID 不正确。 第二个方案涉及与 Active Directory 组织单位 (OU) 的目录同步。 如果用户已登录到 SharePoint, 然后将移动到不同的 OU 并 resynced 使用 SharePoint, 他们可能会遇到此问题。

1. 若要解决此问题, 您应使用本文中的步骤还原原始 UPN, 在[Office 365 中还原用户](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)。
2. 如果无法还原原始用户, 则应使用这些步骤从 OneDrive 网站中删除旧用户, 并[从 "用户信息" 列表中删除用户]()。 
3. 完成此操作后, 您可以通过按照为[用户的 Onedrive 添加管理员的](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)步骤来验证用户是否具有对 onedrive 网站的管理员权限。

有关权限级别的详细信息, 请参阅[了解 SharePoint 中的权限级别](https://docs.microsoft.com/sharepoint/understanding-permission-levels)一文。
