---
title: API 权限和许可
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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932087"
---
# <a name="api-permissions-and-consent"></a>API 权限和许可

与应用程序集成Microsoft 标识平台遵循授权模型，使用户和管理员能够控制如何访问数据。 授权模型的实现已在 Microsoft 标识平台 终结点上更新。 它会更改应用必须与应用交互Microsoft 标识平台。 [Microsoft 标识平台](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)终结点中的权限和同意涵盖此授权模型的基本概念，包括范围、权限和同意。

借助[Azure Active Directory (Azure AD) 框架](https://docs.microsoft.com/azure/active-directory/develop/consent-framework)，可以轻松开发多租户 Web 和本机客户端应用程序。 这些应用程序允许用户帐户从 Azure AD 租户登录，该租户不同于注册应用程序的租户。 除了你自己的 Web API 之外，他们还需要访问 Web API（如 Microsoft Graph API (）来访问 Microsoft 365) 和其他 Microsoft 服务 API 中的 Azure AD、Intune 和服务。

