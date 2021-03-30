---
title: '配置 SSO (无缝单一) '
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
- "9004344"
- "9004357"
- "9384"
- "9863"
ms.openlocfilehash: bd3873c2db1b8d548f81d531a8bf5747130fe761
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402257"
---
# <a name="configure-seamless-single-sign-on-sso"></a>配置 SSO (无缝单一) 

**配置应用程序**

1. 您应从应用程序供应商获取值。 您可以手动输入值或上载元数据文件以提取字段的值。
2. 许多应用已预配置为与 Azure AD 一起运行。 这些应用在将应用添加到 Azure AD 租户时可浏览的应用库中列出。 [快速入门系列](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure)将引导你完成此过程。
3. 若要创建非库应用程序，可以单击 **" +** 创建你自己的应用程序"按钮，然后为应用程序命名。
    - 默认情况下， **它将选择"** 集成在库中找不到的其他任何应用程序"，这是非库应用程序的正确选项。
    - 一 **旦在输入** 应用程序的名称后点击"创建"，它将创建一个新的非库企业应用程序。
    - 然后，你可以导航到"管理该应用程序"下的"单一登录"，并且你将能够看到用于在你的环境中实现它的不同技术。

**为特定应用程序配置无缝 SSO**

对于库中的应用，你将找到详细的分步说明。 若要访问这些步骤，你可以浏览 SaaS 应用配置教程中所有应用 [配置教程的列表](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)。

**配置基于 SAML 的 SSO**

1. [快速入门：为 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-sso) (Azure AD) 租户中的应用程序设置基于 SAML 的单一登录 (S) SO) 。
2. 若要了解有关单一登录的基于 SAML 的选项，请参阅了解基于 [SAML 的单一登录](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-saml-single-sign-on)。
3. 若要了解 Azure Active Directory (Azure AD) 支持单一 Sign-On (SSO) 的 SAML 2.0 身份验证请求和响应，请参阅 [单一 Sign-On SAML 协议](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)。
4. 若要了解如何使用 Microsoft Graph API 为 Azure Active Directory (Azure AD) 中的应用程序创建和配置基于 SAML 的单一登录 (SSO) ，请参阅使用 Microsoft Graph API 为应用程序配置基于 [SAML](https://docs.microsoft.com/graph/application-saml-sso-configure-api)的单一登录。
5. 若要了解 Azure AD 如何使用 SAML 协议，请参阅 [Microsoft 标识平台如何使用 SAML 协议](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-protocol-reference)。

**配置令牌和声明**

1. [如何：自定义在企业应用程序的 SAML 令牌中颁发的声明](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)。
2. 若要了解如何使用 PowerShell 配置声明，请参阅如何：自定义在租户中的特定应用的令牌中发出的声明 ([预览 ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)) 。
3. 若要了解如何配置可选声明，请参阅 [如何：向应用提供可选声明](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)。
4. 若要了解如何使用目录架构扩展属性将用户数据发送到令牌声明中的应用程序，请参阅使用声明中的目录 [架构扩展属性](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions)。
5. 若要了解如何配置令牌生存期，请参阅 Microsoft 标识平台中的可配置令牌 ([预览) 。 ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes)
6. [Configure token lifetime policies (preview) ](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes) - 本文将介绍一个常见的策略方案，可帮助您为令牌生存期实施新规则。 在示例中，您将了解如何创建要求用户在 Web 应用中更频繁地进行身份验证的策略。

**SSO 配置疑难解答**

- 有关 Azure Active Directory 无缝单一Sign-On (无缝 SSO) 的常见问题，请参阅 [Azure Active Directory 无缝单一登录：常见问题](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq)。
- 有关 Azure Active Directory (Azure AD) 无缝单一 Sign-On (无缝 SSO) 的常见问题的疑难解答信息，请参阅 Azure [Active Directory 无缝单一登录疑难解答](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso)。
