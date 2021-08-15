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
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993883"
---
# <a name="delete-tenant"></a>删除租户

若要删除 Azure AD，请确保：
- 你是目录上的全局管理员。
- 你未使用默认目录的帐户登录，例如 contoso.onmicrosoft.com 登录帐户（如 admin@contoso.onmicrosoft.com）。
- 删除之前删除目录中的任何活动应用程序。 若要删除活动应用程序，请导航到"应用注册"并删除现有应用程序。
- 没有任何活动订阅适用于任何Microsoft Online Services，例如Microsoft Azure、Office 365或Azure AD Premium关联的订阅。 通过 Azure 支持和计费转移订阅或加速取消活动订阅。 详细了解如何取消 Office 365 和 Azure 订阅。 有关将现有订阅关联或添加到租户的指南，请参阅将 Azure 订阅关联或添加到 [Azure AD 租户](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)。
- 没有活动许可证。 若要删除许可证，请参阅 [如何删除订阅以删除许可证](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)。
- 在尝试删除 Azure AD 时，目录中除您自己作为全局管理员外，没有任何其他活动用户。 删除任何其他活动用户，并且还需要删除租户中自定义域名的任何依赖项，例如使用 admin@contoso.com。

有关如何执行下列操作的详细信息步骤：
- 删除"Azure Active Directory"或"订阅"，请参阅[删除Azure Active Directory。](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)
- 删除目录中的应用程序，请参阅 [删除应用程序](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app)。 
