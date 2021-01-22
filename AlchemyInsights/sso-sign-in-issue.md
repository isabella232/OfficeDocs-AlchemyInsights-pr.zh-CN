---
title: 无缝 SSO 用户登录问题
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
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/21/2021
ms.locfileid: "49919197"
---
# <a name="seamless-sso-user-sign-in-issues"></a>无缝 SSO 用户登录问题

对用户进行身份验证后，浏览器将缓存用户的凭据，以便在同一浏览器中，应用程序将自动使用同一帐户登录。 这可能会导致另一个用户或单个用户难以登录到一台设备上的多个帐户。 若要解决此问题：1. 尝试在另一个浏览器上登录。 2. 清除浏览器的缓存和/或 Cookie，然后再次尝试登录。

如果仍遇到登录问题，我们建议执行下列操作来诊断和自动执行解决方案步骤：

1. 安装 ["我的应用](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) "安全浏览器扩展，以帮助 Azure Active Directory (Azure AD) ，以在使用 Azure 门户中的测试体验时提供更好的诊断和解决方案。
2. 在 Azure 门户的应用配置页面中使用测试体验重现错误。 若要了解更多信息，请参阅 [调试基于 SAML 的单一登录应用程序](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)。
3. 如果你将 Azure 门户中的测试体验与"我的应用"安全浏览器扩展一同使用，可以跳过步骤 **4。**
4. 若要打开基于 SAML 的单一登录配置页面：
    - 打开 [Azure 门户](https://portal.azure.com/)，以全局管理员 **或****Coadmin 登录**。
    - 通过选择 **左侧主导航** 菜单顶部的"所有服务"打开 Azure Active Directory 扩展。
    - 在筛选器搜索框中键入"Azure Active Directory"，然后选择 **Azure Active Directory** 项。
    - 从 **Azure** Active Directory 左侧导航菜单中选择企业应用程序。
    - 选择 **"所有** 应用程序"以查看所有应用程序的列表。 如果在此处看不到要显示的应用程序，请使用"所有应用程序"列表顶部的筛选器控件，将"显示"选项设置为"**所有应用程序"。** 
    - 选择要为单一登录配置的应用程序。
    - 加载应用程序后，从应用程序的左侧导航菜单中选择"单一登录"。
    - 选择 **基于 SAML 的 SSO。**
5. 根据该错误，若要了解有关要遵循的建议步骤的详细信息，请参阅"登录到基于 SAML 的单一[登录配置的应用时遇到问题"。](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)
6. 若要解决其他用户的登录问题，请参阅以下指南：
    - [单Sign-On SAML 协议](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [如何：使用 Azure Active Directory 报告排查登录错误](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [意外同意提示](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [用户同意错误](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [从"我的应用程序"登录时出现问题](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [应用程序登录页上的错误](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [登录 Microsoft App 时出现问题](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
