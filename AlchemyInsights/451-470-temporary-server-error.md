---
title: 451 4.7.0 临时服务器错误。 请稍后重试。 PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918961"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 临时服务器错误。 请稍后重试。 PRX4

在使用 SMTP 客户端提交方法通过 Smarthost"smtp.office365.com"发送电子邮件时，您可能会面临问题，并收到错误："451 4.7.0 临时服务器错误。 请稍后重试。 PRX4 主要是临时的。" 

确保没有将共享邮箱用于 SMTP 客户端提交，因为 SMTP 客户端的 Submission 方法需要经过许可的邮箱来发送邮件。 但是，如果您未使用共享邮箱且问题仍然存在，请检查以下内容：

1. 通过运行此 PowerShell 命令，在正使用的许可邮箱上启用客户端 SMTP 提交：

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    或

    1. 转到"Microsoft 365 管理中心 >**活动用户"，** 然后选择该用户。
    1. 转到"邮件"选项卡 **>"电子邮件>** 选择"**管理电子邮件应用程序"。** 
    1. 确保选中 **"已验证的 SMTP"** 设置 (启用) 。
    1. 选择“**保存更改**”。
    
    若要为整个组织启用 SMTP 身份验证，请运行此命令：

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **注意**：出于安全原因，建议仅为所使用的邮箱启用 SMTP 身份验证。 用户级别设置会覆盖组织级别设置。

2. 通过切换"启用安全默认值"禁用 Azure安全性默认值，设置为 **"否"：**

    1. 以安全管理员、条件访问管理员或全局管理员登录 Azure 门户。
    1. 浏览到Azure Active Directory >**  属性**"，然后选择 **"管理安全性默认值"。**
    1. 将 **"启用安全默认值"开关** 设置为"**否"。**
    1. 选择“**保存**”。

3. 禁用使用 (邮箱) 多重身份验证和 MFA 身份验证。

    1. 转到"Microsoft 365 管理中心"，在左侧导航菜单中选择 **"用户""**  >  **活动用户"。**
    1. 在“**活动用户**”页面上，选择“**多重身份验证**”。
    1. 选择用户并禁用 **多重身份验证**。

