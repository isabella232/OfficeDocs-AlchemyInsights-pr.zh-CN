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
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="b9bc4-102">令牌声明和属性的问题</span><span class="sxs-lookup"><span data-stu-id="b9bc4-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="b9bc4-103">**更新、配置或删除令牌声明**</span><span class="sxs-lookup"><span data-stu-id="b9bc4-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="b9bc4-104">通过使用 Azure Active Directory (Azure AD) ，可以在[](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management)授权应用后收到的响应令牌中自定义角色声明声明的类型。</span><span class="sxs-lookup"><span data-stu-id="b9bc4-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="b9bc4-105">应用程序开发人员可以在其 Azure AD 应用程序中使用可选声明，以指定他们在发送到其应用程序的令牌中需要哪些声明。</span><span class="sxs-lookup"><span data-stu-id="b9bc4-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="b9bc4-106">有关详细信息，请参阅"[为应用提供可选声明"。](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="b9bc4-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="b9bc4-107">[使用 Azure Active Directory 为应用程序配置组声明](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)。</span><span class="sxs-lookup"><span data-stu-id="b9bc4-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="b9bc4-108">如果在应用程序中使用无缝单一登录，请参阅自定义在企业应用程序的 [SAML 令牌中颁发的声明](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)。</span><span class="sxs-lookup"><span data-stu-id="b9bc4-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="b9bc4-109">**声明属性映射**</span><span class="sxs-lookup"><span data-stu-id="b9bc4-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="b9bc4-110">若要使用 PowerShell 配置声明映射策略，请参阅自定义在租户预览版中为特定应用 (令牌[) 。 ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)</span><span class="sxs-lookup"><span data-stu-id="b9bc4-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="b9bc4-111">目录架构扩展属性提供了一种在用户对象和其他目录对象（如组、租户详细信息、服务主体）上存储 Azure Active Directory 中其他数据的方法。</span><span class="sxs-lookup"><span data-stu-id="b9bc4-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="b9bc4-112">只能使用用户对象上的扩展属性将声明发出到应用程序。</span><span class="sxs-lookup"><span data-stu-id="b9bc4-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="b9bc4-113">[在声明中使用目录](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) 架构扩展属性描述如何使用目录架构扩展属性将用户数据发送到令牌声明中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="b9bc4-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="b9bc4-114">有关令牌声明详细信息，请参阅：</span><span class="sxs-lookup"><span data-stu-id="b9bc4-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="b9bc4-115">访问令牌中的声明</span><span class="sxs-lookup"><span data-stu-id="b9bc4-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="b9bc4-116">应用程序中的id_token</span><span class="sxs-lookup"><span data-stu-id="b9bc4-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="b9bc4-117">[可以在](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) Azure AD B2C 颁发的 ID 令牌和访问令牌中预期声明</span><span class="sxs-lookup"><span data-stu-id="b9bc4-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="b9bc4-118">SAML 令牌声明引用</span><span class="sxs-lookup"><span data-stu-id="b9bc4-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
