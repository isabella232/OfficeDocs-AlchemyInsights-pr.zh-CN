---
title: 对 OneDrive for Business 网站的 "拒绝访问" 消息进行故障排除
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670606"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>对 OneDrive for Business 网站的 "拒绝访问" 消息进行故障排除

在使用相同的用户主体名称 (UPN) 中删除并重新创建用户时，通常会出现此问题。 新帐户是使用其他 PUID (Passport 唯一 ID) 值创建的。 当用户尝试访问网站集或其 OneDrive 时，用户的 PUID 不正确。 第二个方案涉及目录与 Active Directory 组织单位 (OU) 的同步。 如果用户已登录到 SharePoint，然后将移动到不同的 OU 并 resynced 使用 SharePoint，他们可能会遇到此问题。

1. 若要解决此问题，您应使用本文中的步骤还原原始 UPN，在 [Microsoft 365 中还原用户](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)。
2. 如果无法还原原始用户，则应使用这些步骤从 OneDrive 网站中删除旧用户，并 [从 "用户信息" 列表中删除用户]()。 
3. 完成此操作后，您可以通过按照为[用户的 Onedrive 添加管理员的](https://docs.microsoft.com/sharepoint/manage-user-profiles)步骤来验证用户是否具有对 onedrive 网站的管理员权限。

有关权限级别的详细信息，请参阅 [了解 SharePoint 中的权限级别](https://docs.microsoft.com/sharepoint/understanding-permission-levels)一文。
