---
title: 凭据问题
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052943"
---
# <a name="issues-with-credentials"></a>凭据问题

[Microsoft 标识平台和 OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 客户端凭据流描述如何直接针对 OAuth 2.0 客户端凭据授予流进行编程。

**如何管理应用程序的密码或证书凭据？**

在 Azure CLI 中，可以使用 [az 广告](https://docs.microsoft.com/cli/azure/ad/app/credential) 应用凭据删除、列出或重置应用程序的密码或证书凭据。

**我的用户如何重置其密码？**

用户需要 [先注册自助服务密码重置](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) ，然后才能重置其密码。 用户注册后，可以按照本文中的说明重置其密码：重置 [工作或学校密码](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)。

**我的用户如何更改其密码？**

用户可以按照本文中的步骤更改其密码： [如何更改密码](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)。
他们还可以 [管理应用密码进行两步验证](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)。

**我的用户在更改或重置密码时收到错误**

此链接将提供有关用户尝试重置其密码时可能出现的常见问题的信息：常见问题 [及其解决方案](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**重置用户密码时遇到问题**

- 请确保你有权重置密码。 *只有全局、密码和用户管理员可以重置用户密码。* 全局管理员还可以重置其他特权管理员的密码。

- 确保您了解许可要求：

  - 必须在组织中分配至少一个许可证：
    - **仅云用户** - 任何 Office 365 (O365) 付费 SKU 或 Azure AD Basic
    - **云和/或** 本地用户 - Azure AD Premium P1 或 P2、企业移动性 + 安全性 (EMS) 或 Secure Productive Enterprise (SPE) 
    - 若要了解有关许可要求的信息，请参阅 [Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)自助服务密码重置的许可要求。
- 若要重置用户密码，在 Azure AD 中查找用户。 然后，在该用户的概述边栏选项卡上，单击"重置密码"按钮。

**密码重置按钮灰出**

您 **无权重置此** 用户的密码。 *只有全局、密码和用户管理员可以重置用户密码。* 全局管理员还可以重置其他特权管理员的密码。

**我看不到密码重置边栏选项卡**

您无权重置密码。 *只有全局、密码和用户管理员可以重置用户密码。* 全局管理员还可以重置其他特权管理员的密码。

**在密码重置中看不到本地集成边栏选项卡**

- 本地集成边栏选项卡仅出现在混合环境中 - 这意味着你正在使用密码写回操作本地用户的密码。

- 如果：

  - 您没有使用密码写回
  - 密码写回的安装/连接存在问题
  - Azure AD Connect 的安装/连接存在问题
  - 有关密码写回问题的更多疑难解答步骤，请参阅 [密码写回疑难解答](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**不知道如何重置用户密码**

1. 以适当的管理员登录 Azure 门户。
2. 转到"**用户和组"** 边栏选项卡，选择 **"所有用户"。**
3. 从列表中选择用户。
4. 对于所选用户，选择 **"概述**"，然后在命令栏中，选择"**重置密码"。**
5. 选择 **"重置密码"** 按钮并按照屏幕上的说明操作。
    - 仅通过 Azure 门户执行的 **重置** 支持密码写回。

**我在 Office 365 管理门户或 Office 365 移动应用程序中重置本地用户的密码，但该用户仍无法登录**

此门户不支持密码写回。 在 Azure 门户中再次重置用户密码。
