---
title: 'SAML 断言 (令牌) '
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
- "9004341"
- "7753"
ms.openlocfilehash: 9c8ff0d4ff6da98ed6a5c42570d4a5fac80b00e93d1356b298528bd8d2c51a5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109230"
---
# <a name="saml-assertions-tokens"></a>SAML 断言 (令牌) 

1. 安全声明标记语言 (SAML) 令牌是声明的 XML 表示形式。 默认情况下，联合安全Windows中 (WCF) 的 SAML 令牌是颁发令牌。 有关详细信息，请参阅 [SAML 令牌和声明](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)。
2. 应用程序Microsoft 标识平台处理每个身份验证流时发出多种类型的安全令牌。 [SAML 令牌声明引用](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) 介绍了 SAML 2.0 令牌的格式、安全特征和内容。
3. 请按照中可[配置的令牌生存期中的](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)Microsoft 标识平台了解如何配置令牌生存期。
4. 按照本文中概述 [的步骤操作](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) ，了解如何配置 Azure AD SAML 令牌加密。
5. 在 Azure AD 中，你可以设置证书签名选项和证书签名算法。 有关详细信息，请参阅[SAML 令牌](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)中适用于库应用的高级证书签名Azure Active Directory。
