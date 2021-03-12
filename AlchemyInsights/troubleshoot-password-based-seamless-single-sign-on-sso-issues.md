---
title: 解决基于密码的无缝单一登录 (SSO) 问题
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
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709491"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>解决基于密码的无缝单一登录 (SSO) 问题

若要了解基于密码的 SSO 的基础，请参阅 [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)基于密码的身份验证。

**配置基于密码的 SSO**

1. [配置基于密码的单一登录](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - 本文详细介绍了基于密码的 SSO 选项。 如果要添加的应用程序需要自定义配置，并且需要使用基于密码的 SSO，则本文适合您。
2. [为本地应用](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) 配置基于密码的单一登录 - 应用程序代理支持多种单一登录模式。 基于密码的登录适用于使用用户名/密码组合进行身份验证的应用程序。 为应用程序配置基于密码的登录时，用户必须登录本地应用程序一次。 此后，Azure Active Directory 将存储登录信息，并会在用户访问它时自动向应用程序提供此信息。
    - 你应该已经使用应用程序代理发布和测试应用。 如果没有，请按照使用 Azure [AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) 应用程序代理发布应用程序中的步骤操作，然后继续为 Prem 应用配置基于密码的 SSO。

若要对基于密码的 SSO 进行疑难解答，请参阅 Azure AD 中基于密码的单 [一登录疑难解答](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
