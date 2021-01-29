---
title: 配置和自定义应用程序
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
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/29/2021
ms.locfileid: "50043977"
---
# <a name="configure-and-customize-applications"></a>配置和自定义应用程序

**配置应用程序**

1. [快速入门：在 Azure Active Directory (Azure AD) ](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) 中配置应用程序的属性，可展示如何为应用配置一些属性。
2. 为了帮助将应用程序与 Azure Active Directory 集成，[](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)我们开发了教程集合，指导你完成配置。
3. [如何配置应用程序代理应用程序](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) 可帮助您了解如何在 Azure AD 中配置应用程序代理应用程序，以将本地应用程序公开到云中。
4. [下载 PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)并配置应用程序：按照为 *Azure AD 配置 PingAccess* 中的说明保护在 Ping Identity 网站上使用 Microsoft Azure AD 应用程序代理发布的应用程序，并下载最新版本的 PingAccess。

**AADSTS650056 (错误的应用程序) 错误**

1. 确保从应用程序所有者提供的登录地址访问应用程序。 否则，请通过正常过程登录到应用程序。 在大多数情况下，这可自动自动解决。 如果没有，则此文章可帮助进行疑难解答和解决。
2. **如果组织拥有该应用程序 (** 则意味着应用程序注册位于组织) ：
    - 建议至少添加来自 Microsoft `User.Read` `openid` **Graph** 的或委派的权限。
    - 确保应用程序及其所有权限都得到同意。 可以通过查看 API 权限中应用程序注册的状态列来 **验证这一点**。
    - 在某些情况下，应用程序可能是第三方，但它可能在组织中注册。 确认此应用程序是否列在应用注册中 (不是企业) 。
    - 如果继续看到此错误消息。 然后，你可能需要生成步骤 **4** 中所述的同意 URL。
3. **如果你的组织不是应用程序所有者，并使用它作为第三方应用程序：**
    - 如果你是全局/公司管理员，你应该会看到同意屏幕。 请确保选中"代表你的组织 **同意"框**。
    - 如果看不到许可屏幕，请删除企业应用程序，然后重试。
    - 如果继续看到此错误消息。 然后，你可能需要生成步骤 **4** 中所述的同意 URL。
4. 手动生成要使用的同意 **URL：** 如果应用程序旨在访问特定资源，你可能无法从 Azure 门户使用"同意"按钮，你将需要手动生成自己的同意 URL 并使用此 URL。
    - 你将需要从 `{App-Id}` 应用程序所有者 `{App-Uri-Id}` 获取和获取。 `{Tenant-Id}` 将成为你的租户标识符。 这将是或 `yourdomain.onmicrosoft.com` 你的目录 ID。
    - 如果应用程序正在访问资源本身，则 `{App-Id}` and `{App-Uri-Id}` 将相同。
5. 有关详细信息，请参阅登录到基于 SAML 的单一 [登录配置的应用时出现问题](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)。

**自定义应用程序**

- 将品牌添加到组织的[Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding)登录页面 - 使用组织的徽标和自定义配色方案为 Azure Active Directory (Azure AD) 登录页面提供一致的外观。
- [使用 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) 门户添加自定义域名 - 每个新的 Azure AD 租户都附带一个初始域名。 不能更改或删除初始域名，但可以添加组织的名称。 添加自定义域名可帮助您创建用户熟悉的用户名。
