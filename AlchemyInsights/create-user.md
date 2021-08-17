---
title: 创建用户
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: afba00ffc6ba082606e0071b41e2917b11e6a39d61cd0df7e468f0238f2ed8e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118734"
---
# <a name="create-user"></a>创建用户

**公告：**

- [从 Google 自 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) 年 1 月 4 日起弃用 WebView 登录支持。 按照 Google 有关测试兼容性的指南测试 [你的应用是否可能](https://go.microsoft.com/fwlink/?linkid=2157323) 受到影响。
- 请确保在使用 Google 使用者帐户登录用户时，使用系统 Web 视图或系统浏览器。 有关详细信息，请参阅[仅使用 Chrome 浏览器登陆应用的问题](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)。

**我无法在我的 Azure AD 目录中创建新用户**

1. 确保你具有创建新的标准用户的权限。 只有 AD 管理员中的全局管理员Azure Active Directory (用户) 才能创建新的标准用户。 如果你不属于上述角色，需请求管理员将你添加到某个上述角色，或让他们为你创建新的用户账户。
1. 确保域中的用户名在你的 Azure AD 中完成过验证。 如果你在 Azure AD 中没有任何验证过的自定义域名，你可以使用以 *.onmicrosoft.com 结尾的 Azure AD 初始域名。
1. 确保用户名所在域不是从你的本地 AD 上与 Azure AD 联合的域。 无法使用从本地联合的域名将用户添加到云。
1. 确保没有其他用户或联系人已经使用了你想要分配给新用户的用户名。 用户名必须是 Azure AD 中唯一的。
1. 参阅你的 Azure AD 的 [Azure AD 角色和管理员](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)。
1. 参阅你的 Azure AD 的[域名](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)。
1. 检查 [审核日志](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) 来查看关于最近创建的或删除的用户的详细信息，比如谁执行的操作以及何时执行的。
1. 有关添加新用户的信息，请参阅使用 Azure 门户在 [Azure AD 中创建新用户](/azure/active-directory/active-directory-users-create-azure-portal)。
1. [Azure AD 管理角色](/azure/active-directory/active-directory-assign-admin-roles)：管理员角色权限Azure Active Directory
1. 您还可以使用 [Azure AD PowerShell 创建新用户](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)。
