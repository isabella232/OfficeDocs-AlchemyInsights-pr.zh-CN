---
title: 对拒绝访问网站OneDrive for Business疑难解答
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957783"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>对拒绝访问网站OneDrive for Business疑难解答

此问题最常发生在使用与 UPN 帐户相同的用户主体名称删除 (时) 。 通过使用不同的 PUID 和 Passport 唯一 ID (值创建) 帐户。 当用户尝试访问网站集或OneDrive时，用户的 PUID 不正确。 第二个方案涉及与 ACTIVE Directory 组织单位和 OU (进行) 。 如果用户已登录到 SharePoint，然后移至其他 OU，然后使用 SharePoint 重新同步，则可能会遇到此问题。

1. 若要解决此问题，应该按照文章还原用户中的步骤还原原始 UPN [Microsoft 365。](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)
2. 如果无法还原原始用户，则应该使用以下步骤从 OneDrive 网站中删除旧用户，从用户信息[列表中删除用户]()。 
3. 完成此操作后，可以按照为用户的网站添加管理员的步骤验证用户是否具有 OneDrive[网站的管理员OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

有关权限级别详细信息，请参阅了解用户权限[级别](https://docs.microsoft.com/sharepoint/understanding-permission-levels)SharePoint。
