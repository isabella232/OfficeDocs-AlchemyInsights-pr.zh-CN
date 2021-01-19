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
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884558"
---
# <a name="saml-assertions-tokens"></a>SAML 断言 (令牌) 

1. 安全声明标记语言 (SAML) 令牌是声明的 XML 表示形式。 默认情况下，在联合安全 (使用的 WCF) SAML 令牌将颁发令牌。 有关详细信息，请参阅 [SAML 令牌和声明](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)。
2. Microsoft 标识平台在处理每个身份验证流时发出多种类型的安全令牌。 [SAML 令牌声明引用](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) 描述 SAML 2.0 令牌的格式、安全特征和内容。
3. 按照 Microsoft 标识平台中可 [配置的令牌生存期中的指南](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) 了解如何配置令牌生存期。
4. 按照本文中概述 [的步骤](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) 了解如何配置 Azure AD SAML 令牌加密。
5. 在 Azure AD 中，你可以设置证书签名选项和证书签名算法。 有关详细信息，请参阅 Azure Active Directory 中库应用的 SAML 令牌中的高级 [证书签名选项](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)。
