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
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50029975"
---
# <a name="issues-with-token-claims-and-attributes"></a>令牌声明和属性的问题

**更新、配置或删除令牌声明**

1. 通过使用 Azure Active Directory (Azure AD) ，可以在[](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)授权应用后收到的响应令牌中自定义角色声明声明的类型。
2. 应用程序开发人员可以在其 Azure AD 应用程序中使用可选声明，以指定他们在发送到其应用程序的令牌中需要哪些声明。 有关详细信息，请参阅"[为应用提供可选声明"。](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [使用 Azure Active Directory 为应用程序配置组声明](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)。
4. 如果在应用程序中使用无缝单一登录，请参阅自定义在企业应用程序的 [SAML 令牌中颁发的声明](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)。

**声明属性映射**

1. 若要使用 PowerShell 配置声明映射策略，请参阅自定义在租户预览版中为特定应用 (令牌[) 。 ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)
2. 目录架构扩展属性提供了一种在用户对象和其他目录对象（如组、租户详细信息、服务主体）上存储 Azure Active Directory 中其他数据的方法。 只能使用用户对象上的扩展属性将声明发出到应用程序。 [在声明中使用目录](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) 架构扩展属性描述如何使用目录架构扩展属性将用户数据发送到令牌声明中的应用程序。

有关令牌声明详细信息，请参阅：

- [访问令牌中的声明](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [应用程序中的id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [可以在](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) Azure AD B2C 颁发的 ID 令牌和访问令牌中预期声明
- [SAML 令牌声明引用](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
