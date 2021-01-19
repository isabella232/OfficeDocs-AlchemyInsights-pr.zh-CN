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
# <a name="saml-assertions-tokens"></a><span data-ttu-id="f9e83-102">SAML 断言 (令牌) </span><span class="sxs-lookup"><span data-stu-id="f9e83-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="f9e83-103">安全声明标记语言 (SAML) 令牌是声明的 XML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9e83-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="f9e83-104">默认情况下，在联合安全 (使用的 WCF) SAML 令牌将颁发令牌。</span><span class="sxs-lookup"><span data-stu-id="f9e83-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="f9e83-105">有关详细信息，请参阅 [SAML 令牌和声明](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)。</span><span class="sxs-lookup"><span data-stu-id="f9e83-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="f9e83-106">Microsoft 标识平台在处理每个身份验证流时发出多种类型的安全令牌。</span><span class="sxs-lookup"><span data-stu-id="f9e83-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="f9e83-107">[SAML 令牌声明引用](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) 描述 SAML 2.0 令牌的格式、安全特征和内容。</span><span class="sxs-lookup"><span data-stu-id="f9e83-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="f9e83-108">按照 Microsoft 标识平台中可 [配置的令牌生存期中的指南](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) 了解如何配置令牌生存期。</span><span class="sxs-lookup"><span data-stu-id="f9e83-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="f9e83-109">按照本文中概述 [的步骤](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) 了解如何配置 Azure AD SAML 令牌加密。</span><span class="sxs-lookup"><span data-stu-id="f9e83-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="f9e83-110">在 Azure AD 中，你可以设置证书签名选项和证书签名算法。</span><span class="sxs-lookup"><span data-stu-id="f9e83-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="f9e83-111">有关详细信息，请参阅 Azure Active Directory 中库应用的 SAML 令牌中的高级 [证书签名选项](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)。</span><span class="sxs-lookup"><span data-stu-id="f9e83-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
