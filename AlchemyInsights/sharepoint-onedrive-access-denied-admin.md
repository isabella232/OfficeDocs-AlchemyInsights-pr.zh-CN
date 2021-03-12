---
title: 访问被拒绝邮件疑难解答
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707944"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>排查 Sharepoint/OneDrive 管理中心中拒绝访问的消息

如果在尝试浏览到 Sharepoint/OneDrive 管理中心时收到拒绝访问消息，请确保向用户分配 [许可证](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)。 如果用户拥有许可证，则还应确保为其分配了可以访问管理中心的管理员[](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles)角色。

在 UPN 服务器中删除用户并使用相同的用户主体名称重新创建用户时， (也会) 。 通过使用不同的 PUID 和 Passport 唯一 ID (值创建) 帐户。 当用户尝试访问网站集或 OneDrive 时，用户的 PUID 不正确。 第二个方案涉及与 ACTIVE Directory 组织单位或 OU (的目录) 。 如果用户已登录 SharePoint，然后移至其他 OU 并与 SharePoint 重新同步，则可能会遇到此问题。

若要解决此问题，您应使用文章"在 [Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)中还原用户"中的步骤还原原始 UPN。

注意：如果 OneDrive 或 SharePoint 管理中心对以前具有访问权限的多个用户不可用，则可能是临时服务问题。  [检查服务运行状况仪表板](https://portal.office.com/adminportal/home#/servicehealth)。


