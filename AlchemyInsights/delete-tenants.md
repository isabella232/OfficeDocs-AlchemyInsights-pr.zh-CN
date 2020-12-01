---
title: 删除租户
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477647"
---
# <a name="delete-tenant"></a>删除租户

若要删除 Azure AD，请确保：
- 您是目录的全局管理员。
- 您未使用在登录帐户中具有默认目录（如 contoso.onmicrosoft.com）的帐户登录，如 admin@contoso.onmicrosoft.com。
- 删除前删除目录中所有活动的应用程序。 若要删除活动的应用程序，请导航到 "应用注册" 并删除现有的应用程序。
- 没有任何 Microsoft Online Services 的活动订阅，例如 Microsoft Azure、Office 365 或与目录关联的 Azure AD Premium。 通过 Azure 支持和帐单转移订阅或加快活动订阅的取消。 了解有关如何取消 Office 365 和 Azure 订阅的详细信息。 有关将现有订阅关联或添加到租户的指南，请参阅 [将 azure 订阅关联或添加到 AZURE AD 租户](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)。
- 没有活动的许可证。 若要删除许可证，请参阅 how [to Remove 订阅 To remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)。
- 在尝试删除 Azure AD 时，目录中没有其他任何活动用户，而是将自己作为全局管理员。 删除任何其他活动用户，同时还需要删除租户中的自定义域名的任何依赖项，如使用 admin@contoso.com 创建的用户。

有关如何执行以下操作的更多详细步骤：
- 删除 "Azure Active Directory" 或 "订阅"，请参阅 [删除 Azure Active directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)。
- 删除目录中的应用程序，请参阅 [删除应用程序](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app)。 
