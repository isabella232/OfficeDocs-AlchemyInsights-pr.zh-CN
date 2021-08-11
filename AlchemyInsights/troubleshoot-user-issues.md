---
title: 用户问题疑难解答
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7813"
- "9004358"
ms.openlocfilehash: 0c4ee54a6f1d00e7fd3794539ba185afa4327af1124d8057550806f7fa87de7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54092940"
---
# <a name="announcements"></a>公告

关注 Google 关于测试兼容性的指南，测试你的应用受影响的情况。 Google 的指南可以在 https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support 处找到。

确保在使用客户 Google 账户登陆用户时查看了系统的 Web 视图或系统浏览器。 有关详细信息，请参阅[仅使用 Chrome 浏览器登陆应用的问题](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)。


**我无法在我的 Azure AD 目录中创建新用户**

要解决无法在 Azure AD 中创建新用户的问题，执行以下步骤：

1. 确保你具有创建新的标准用户的权限。 只有 Azure Active Directory (AD) 中的全局管理员或用户管理员角色可以创建新的标准用户。 如果你不属于上述角色，需请求管理员将你添加到某个上述角色，或让他们为你创建新的用户账户。
2. 确保域中的用户名在你的 Azure AD 中完成过验证。 如果你在 Azure AD 中没有任何验证过的自定义域名，你可以使用以 *.onmicrosoft.com 结尾的 Azure AD 初始域名。
3. 确保用户名所在域不是从你的本地 AD 上与 Azure AD 联合的域。 无法使用从本地联合的域名将用户添加到云。
4. 确保没有其他用户或联系人已经使用你想要分配给新用户的用户名。用户名在 Azure AD 中必须是唯一的。
5. 参阅你的 Azure AD 的 [Azure AD 角色和管理员](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)。
6. 参阅你的 Azure AD 的[域名](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains)。
7. 检查 [审核日志](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) 来查看关于最近创建的或删除的用户的详细信息，比如谁执行的操作以及何时执行的。
8. 有关添加新用户的详细信息，请参阅[使用 Azure 门户在 Azure AD 中创建新用户](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)。
9. 有关 Azure AD 中管理员角色权限的详细信息，请参阅 [Azure AD 管理角色](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)。
10. 有关使用 Azure AD Powershell 创建用户的详细信息，请参阅[ Azure AD PowerShell 创建新用户](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser)。

**自助注册问题**

要解决自助注册相关问题，执行以下步骤：

1. 要通过应用使用自助注册，首先为你的租户启用自助注册。 
2. 要为应用启用支持自助注册，请将其添加到你的用户流中。 下一次转到应用程序的登录页面时，你将会看到选项“***没有帐户? 创建一个!***” 然后自助注册过程将会开始。
3. 有关如何使用自助注册在 Azure AD 上填充组织，请参阅 [Azure AD 自助注册](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup)。
4. 一旦将用户流与一个或多个应用关联，访问该应用的用户就可以注册并使用在用户流中配置的选项获取来宾账户。 有关注册和获取来宾账户的详细信息，用户可以参阅[来宾用户自助注册](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow)。

**邀请外部用户的有关问题**

要解决邀请外部用户的相关问题，执行以下步骤：

确保你将用户邀请发送到了用户注册时使用的电子邮箱中。 如果你将邀请发送到用户的代理电子邮箱中，用户将无法进行兑换。 有关详细信息，请参阅 [Azure AD B2B 文档](https://docs.microsoft.com/azure/active-directory/external-identities/)。

**我无法将许可证分配给用户**

要解决给用户分配许可证的相关问题，执行以下步骤：

1. 要管理用户许可证，确保你使用的是下列的必需管理员角色账户: 全局管理员、许可证管理员或用户管理员。 你可以在 **目录角色** 选项卡中查看用户的角色。
2. 如果你正在使用 Azure 门户且许可证分配发生故障，请单击右上角的通知按钮。 然后带有错误详细信息的边栏选项卡会打开。 在大多数情况下，它提供了足够供你理解和解决问题的信息。
3. 在完成用户许可证分配之前，确保已经为用户设置好 **使用位置** 属性。 通过查看用户边栏选项卡中的 **个人资料** 选项卡来验证用户的此属性已设置。
4. 确保你将发放的许可证所属的产品有足够多可用的许可证。 你可以在 Azure 门户的 [Azure Active Directory -> 许可证 -> 所有产品](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products)中查看可用的许可证数量。
5. 用户可能已经有了会与你将发送给他们的许可证在服务上相冲突的别的许可证。 比如，如果用户具有 Exchange Online（计划 1）服务，你将不能发送给他们 Exchange Online（计划 2）的许可证。 禁用正在使用的服务来发送新的许可证。 如果你在使用 Azure 门户或 PowerShell cmdlets，**问题详细信息** 页面列出了造成冲突的具体服务。
6. 如果你想要删除发生故障的许可证，用户的其他许可服务可能是依赖于你将要删除的服务的。 如果你在使用 Azure 门户或 PowerShell cmdlets，错误信息将会列出了有依赖关系的具体服务。
7. 如果你想理解为什么某个许可证从用户处被添加/删除（例如，你组织中的谁做出了这样的更改），请查看审核日志。 将筛选器设置为 **许可证活动** 来显示所有的修改，包括执行操作的“主角”。
8. 如果你在使用 Exchange Online，你的租户中的一些用户可能会通过相同的代理地址值被错误地配置。 在这种情况下，你可能会在许可证操作故障时看到一般错误消息。 [这篇文章](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used)包含关于此问题的详细信息，包括[如何使用远程 PowerShell 连接到 Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell) 的信息。要确认租户中的哪些用户包含相同的代理地址，请执行 Exchange Online cmdlet:

运行

Get-Recipient | where {$_.EmailAddresses -match <user principal name>} | fL Name, RecipientType,emailaddresses





