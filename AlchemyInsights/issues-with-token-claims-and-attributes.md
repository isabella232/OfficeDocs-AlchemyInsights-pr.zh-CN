---
title: 令牌声明和属性的问题
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
- "9004347"
- "7761"
ms.openlocfilehash: 0c9827ee312d6b236c86f5a2973fa61fdc78c49b8565dd4ceb41f9a3a48140bc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54012874"
---
# <a name="issues-with-token-claims-and-attributes"></a>令牌声明和属性的问题

**更新、配置或删除令牌声明**

1. 通过使用 Azure Active Directory (Azure AD) ，可以在授权应用后收到的[](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)响应令牌中自定义角色声明声明的类型。
2. 应用程序开发人员可以在其 Azure AD 应用程序中使用可选声明，以指定他们在发送到应用程序的令牌中需要哪些声明。 有关详细信息，请参阅 [向应用提供可选声明](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)。
3. [为应用程序配置组声明Azure Active Directory。](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)
4. 如果在应用程序中使用无缝单一登录，请参阅 [自定义在企业应用程序的 SAML 令牌中颁发的声明](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)。

**声明属性映射**

1. 若要使用 PowerShell 配置声明映射策略，请参阅自定义租户中的特定应用在令牌中发出的声明 ([预览) 。 ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. 目录架构扩展属性提供了一种在用户对象Azure Active Directory（如组、租户详细信息、服务主体）上存储其他数据的方法。 只有用户对象上的扩展属性可用于向应用程序发出声明。 [Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) 介绍如何使用目录架构扩展属性将用户数据发送到令牌声明中的应用程序。

有关令牌声明详细信息，请参阅：

- [访问令牌中的声明](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [a claims in an id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [可以在](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) Azure AD B2C 颁发的 ID 令牌和访问令牌中预期声明
- [SAML 令牌声明引用](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
