---
title: 资源主体或服务主体的问题
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004336"
- "7741"
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028066"
---
# <a name="issues-with-a-resource-or-service-principal"></a>资源主体或服务主体的问题

1. 如果您刚刚开始[，Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)中的应用程序和服务主体对象将介绍 Azure Active Directory 中的应用程序注册、应用程序对象和服务主体：它们是什么、如何使用以及它们如何相互关联。 还介绍了多租户示例方案，以说明应用程序的应用程序对象与相应的服务主体对象之间的关系。
2. 您可以通过读取应用程序中的应用程序和服务主体对象来了解有关应用程序和服务主体之间的关系[Azure Active Directory。](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. How [to： Use the portal to create an Azure AD application and service principal that can access resources](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.
4. 使用 [服务主体 API，](https://docs.microsoft.com/graph/api/resources/serviceprincipal)可以编程方式管理应用程序实例，并控制应用程序可以在租户内执行哪些操作。
5. [servicePrincipal 资源类型](https://docs.microsoft.com/graph/api/resources/serviceprincipal) 列出了 servicePrincipal 资源类型的所有属性和方法。
6. [Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)和 Microsoft Graph 之间的资源类型差异突出显示了 Azure AD Graph 与 Microsoft Graph 之间的差异。 它显示名称不同或不可用的资源;它还突出显示了 Microsoft Graph beta 版本中提供的资源，但不在 v1.0 版本中。

**来宾用户的问题**

- [快速](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) 入门：在 Azure 门户中将来宾用户添加到你的目录将展示如何通过 Azure 门户将新的来宾用户添加到 Azure AD 目录、发送邀请以及查看来宾用户的邀请兑换过程的外观。
- [教程：在 Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows)中创建用户流介绍如何使用 Azure 门户创建一些建议的用户流。 若要了解如何在应用程序中设置资源所有者密码凭据 (ROPC) 流，请参阅在 Azure AD B2C 中配置资源所有者密码凭据流。
