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
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718172"
---
# <a name="create-user"></a>创建用户

**公告：**

- [自 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) 年 1 月 4 日起，Google 弃用 WebView 登录支持。 按照 Google 有关测试兼容性的指导测试 [你的应用是否可能](https://go.microsoft.com/fwlink/?linkid=2157323) 受到影响。
- 请确保在使用消费者 Google 帐户登录用户时使用系统 Webview 或系统浏览器。 有关详细信息，请参阅[仅使用 Chrome 浏览器登陆应用的问题](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)。

**我无法在我的 Azure AD 目录中创建新用户**

1. 确保你具有创建新的标准用户的权限。 只有 Azure Active Directory (AD) 全局管理员或用户管理员角色才能创建新的标准用户。 如果你不属于上述角色，需请求管理员将你添加到某个上述角色，或让他们为你创建新的用户账户。
1. 确保域中的用户名在你的 Azure AD 中完成过验证。 如果你在 Azure AD 中没有任何验证过的自定义域名，你可以使用以 *.onmicrosoft.com 结尾的 Azure AD 初始域名。
1. 确保用户名所在域不是从你的本地 AD 上与 Azure AD 联合的域。 无法使用从本地联合的域名将用户添加到云。
1. 确保没有其他用户或联系人已经使用了你想要分配给新用户的用户名。 用户名必须是 Azure AD 中唯一的。
1. 参阅你的 Azure AD 的 [Azure AD 角色和管理员](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)。
1. 参阅你的 Azure AD 的[域名](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)。
1. 检查 [审核日志](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) 来查看关于最近创建的或删除的用户的详细信息，比如谁执行的操作以及何时执行的。
1. 有关添加新用户的信息，请参阅使用 Azure 门户在 [Azure AD](/azure/active-directory/active-directory-users-create-azure-portal)中创建新用户。
1. [Azure AD 管理角色](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)：Azure Active Directory 中的管理员角色权限
1. 您还可以使用 [Azure AD PowerShell 创建新用户](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)。