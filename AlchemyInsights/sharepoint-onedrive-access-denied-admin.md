---
title: 访问被拒绝邮件疑难解答
ms.author: pebaum
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 4e6fdc6fbf745d1702bf1a7b3474ac82f6662305
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751266"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Sharepoint/OneDrive 管理中心中的拒绝访问邮件疑难解答

如果在尝试浏览到 Sharepoint/OneDrive 管理中心时收到 "拒绝访问" 消息，请确保[将许可证分配](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)给该用户。 如果用户具有许可证，还应确保为其分配可访问管理中心的[管理员角色](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide)。

当用户被删除并重新创建为相同的用户主体名称（UPN）时，也会发生此问题。 使用不同的 PUID （Passport 唯一 ID）值创建新帐户。 当用户尝试访问网站集或其 OneDrive 时，用户的 PUID 不正确。 第二个方案涉及与 Active Directory 组织单位（OU）的目录同步。 如果用户已登录到 SharePoint，然后将移动到不同的 OU 并 resynced 使用 SharePoint，他们可能会遇到此问题。

若要解决此问题，您应使用本文中的步骤还原原始 UPN，在[Office 365 中还原用户](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)。

注意：如果 OneDrive 或 SharePoint 管理中心对之前有权访问的多个用户不可用，则可能存在暂时性的服务问题。  [检查服务运行状况仪表板](https://portal.office.com/adminportal/home#/servicehealth)。


