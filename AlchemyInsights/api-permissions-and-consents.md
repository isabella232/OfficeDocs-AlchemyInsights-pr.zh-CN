---
title: API 权限和同意
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951863"
---
# <a name="api-permissions-and-consent"></a>API 权限和同意

与 Microsoft 标识平台集成的应用程序遵循授权模型，使用户和管理员能够控制如何访问数据。 授权模型的实现已在 Microsoft 标识平台终结点上更新。 它更改应用必须与 Microsoft 标识平台交互的方式。 [Microsoft 标识平台终结点中](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 的权限和许可涵盖此授权模型的基本概念，包括范围、权限和同意。

Azure [Active Directory (Azure AD) 同意框架](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) 使开发多租户 Web 和本机客户端应用程序变得简单。 这些应用程序允许用户帐户从 Azure AD 租户登录，该租户不同于注册应用程序的租户。 除了你自己的 Web API 之外，他们还需要访问 Web API（如 Microsoft Graph API (）来访问 Microsoft 365) 和其他 Microsoft 服务 API 中的 Azure AD、Intune 和服务。

