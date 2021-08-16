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
ms.openlocfilehash: 3ce5b04469eb655c9d682f5830d9f906529aa40f706ee594b670708426d48769
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044978"
---
# <a name="configure-and-customize-applications"></a>配置和自定义应用程序

**配置应用程序**

1. [快速入门：在 Azure AD 租户](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure)中Azure Active Directory (应用程序) 显示如何配置应用的一些属性。
2. 为了帮助将应用程序与Azure Active Directory集成，我们开发了一组[教程](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list)，指导你完成配置。
3. [如何配置应用程序代理应用程序](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) 可帮助你了解如何在 Azure AD 中配置应用程序代理应用程序，以向云公开你的本地应用程序。
4. 下载 [PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)并配置应用程序：按照为 *Azure AD 配置 PingAccess* 中的说明保护在 Ping Identity 网站上使用 Microsoft Azure AD 应用程序代理发布的应用程序，并下载最新版本的 PingAccess。

**AADSTS650056 (配置错误) 错误**

1. 确保从应用程序所有者提供的登录地址访问应用程序。 否则，请通过正常过程登录到应用程序。 在大多数情况下，这可自动自动解决。 如果没有，则此文章可帮助进行疑难解答和解决。
2. **如果你的组织拥有该应用程序 (** 意味着应用程序注册位于你的组织中) ：
    - 建议至少添加 `User.Read` `openid` **Microsoft** Graph委派权限。
    - 确保应用程序及其所有权限都得到同意。 可以通过查看"API 权限"中应用程序注册的"状态"**列来验证这一点**。
    - 在某些情况下，应用程序可能是第三方，但是它可能在组织中注册。 确认"应用程序注册"中是否列出了此应用程序 ("Enterprise应用程序) 。
    - 如果您继续看到此错误消息。 然后，你可能需要构建步骤 **4** 中所述的同意 URL。
3. **如果你的组织不是应用程序所有者，并使用它作为第三方应用程序：**
    - 如果你是全局/公司管理员，你应该会看到同意屏幕。 确保选中"代表 **你的组织同意"框**。
    - 如果看不到许可屏幕，请删除Enterprise应用程序，然后重试。
    - 如果您继续看到此错误消息。 然后，你可能需要构建步骤 **4** 中所述的同意 URL。
4. 手动生成要使用的同意 **URL：** 如果应用程序旨在访问特定资源，你可能无法使用 Azure 门户中的"同意"按钮，你需要手动生成自己的同意 URL 并使用它。
    - 你需要从应用程序 `{App-Id}` 所有者获取 和 `{App-Uri-Id}` 。 `{Tenant-Id}` 将成为你的租户标识符。 这将是 或 `yourdomain.onmicrosoft.com` 目录 ID。
    - 如果应用程序要自行访问资源，则 `{App-Id}` 和 `{App-Uri-Id}` 将相同。
5. 有关详细信息，请参阅登录到基于 SAML 的单一登录配置 [的应用时出现问题](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)。

**自定义应用程序**

- 将品牌添加到组织的[Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding)登录页面 - 使用组织的徽标和自定义配色方案为 Azure Active Directory (Azure AD) 登录页面提供一致的外观。
- [使用自定义门户添加Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) - 每个新的 Azure AD 租户都附带一个初始域名。 不能更改或删除初始域名，但可以添加组织的名称。 添加自定义域名可帮助您创建用户熟悉的用户名。
