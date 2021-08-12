---
title: API 权限和同意流程
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932051"
---
# <a name="api-permissions-and-consent-process"></a>API 权限和同意流程

若要使你的应用可访问 Microsoft Graph 中的数据，用户或管理员必须通过同意过程向其授予正确的权限。 [Microsoft Graph权限参考](https://docs.microsoft.com/graph/permissions-reference)列出了与每个主要 Microsoft 应用程序 API 集Graph的权限。 它还提供有关如何使用权限的指导。

**设置或更新服务主体**

- [Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - 本文演示如何创建新的 servicePrincipal 对象。
- 在门户中创建[Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)服务主体 - 本文演示如何创建新的 Azure Active Directory (Azure AD) 应用程序和服务主体，这些应用程序和服务主体可用于基于角色的访问控制。
- [应用& Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)中的服务主体 - 本文介绍了 Azure Active Directory 中的应用程序注册、应用程序对象和服务主体：它们是什么、如何使用以及它们如何相互关联。

**添加或更新应用注册并提供管理员同意**

- [创建应用注册](https://docs.microsoft.com/graph/api/application-post-applications) - 本文介绍了如何创建新的应用程序对象。
- [更新应用注册 - API 权限](https://docs.microsoft.com/graph/api/application-update) - 本文介绍了如何更新应用程序对象的属性。
- [提供管理员同意](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - 对于管理员同意和同意，我们通常要求管理员明确授予同意。
- [RBAC (beta) ](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - 用于统一角色定义和角色分配的角色管理容器，适用于支持单个 角色分配 中的多个主体和多个作用域的 Microsoft 365 RBAC 提供程序。 这不同于 *rbacApplication* 资源类型。 Microsoft Intune是此类 RBAC 提供程序的一个示例。 Intune 角色分配可以有一个主体数组和一组作用域组。 **This is in beta， meaning that it is still in development and not recommended for use in production.**
