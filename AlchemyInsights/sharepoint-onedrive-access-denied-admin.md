---
title: 拒绝访问邮件疑难解答
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085218"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Sharepoint/OneDrive管理中心中拒绝访问的消息疑难解答

如果在尝试浏览到 Sharepoint/OneDrive管理中心时收到拒绝访问消息，请确保向用户分配[许可证](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)。 如果用户拥有许可证，则还应确保为其分配了可以访问管理中心的管理员[](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles)角色。

在使用 UPN 服务器中删除和重新创建用户时，也会 (此问题) 。 通过使用不同的 PUID 和 Passport 唯一 ID (值创建) 帐户。 当用户尝试访问网站集或OneDrive时，用户的 PUID 不正确。 第二个方案涉及与 ACTIVE Directory 组织单位和 OU (进行) 。 如果用户已登录到 SharePoint，然后移至其他 OU，然后使用 SharePoint 重新同步，则可能会遇到此问题。

若要解决此问题，您应使用文章 Restore [a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)中的步骤还原原始 UPN。

注意：如果OneDrive或SharePoint管理中心对以前具有访问权限的多个用户不可用，则可能是临时服务问题。  [检查服务运行状况仪表板](https://portal.office.com/adminportal/home#/servicehealth)。


