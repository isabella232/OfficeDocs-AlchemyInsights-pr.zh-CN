---
title: 对 OneDrive for Business 网站的 "拒绝访问" 消息进行故障排除
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 42a56b17e41649d979cf442909e8357eb262cf9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35354787"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>对 OneDrive for Business 网站的 "拒绝访问" 消息进行故障排除

在使用相同的用户主体名称 (UPN) 对用户进行删除和重新创建时, 通常会出现此问题。 使用不同的 PUID (Passport 唯一 ID) 值创建新帐户。 当用户尝试访问网站集或其 OneDrive 时, 用户的 PUID 不正确。 第二个方案涉及与 Active Directory 组织单位 (OU) 的目录同步。 如果用户已登录到 SharePoint, 然后将移动到不同的 OU 并 resynced 使用 SharePoint, 他们可能会遇到此问题。

若要解决此问题, 您应使用本文中的步骤还原原始 UPN, 在[Office 365 中还原用户](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)。

完成此操作后, 您可以通过按照为[用户的 Onedrive 添加管理员的](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)步骤来验证用户是否具有对 onedrive 网站的管理员权限。

有关权限级别的详细信息, 请参阅[了解 SharePoint 中的权限级别](https://docs.microsoft.com/sharepoint/understanding-permission-levels)一文。
