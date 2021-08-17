---
title: 启用 SMTP 身份验证和故障排除
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: d16389ca577970deaf743255f75dc86134e79dcab2fff8c33987532fc7ee1105
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57890424"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>启用 SMTP 身份验证和故障排除

如果要为邮箱启用 SMTP 身份验证，或者在尝试通过使用 Microsoft 365 对设备或应用程序进行身份验证来中继电子邮件时收到“客户端未通过身份验证”、“身份验证失败”或“SmtpClientAuthentication”错误消息（代码分别为“5.7.57”、“5.7.3”和“5.7.139”），请执行以下三项操作来解决此问题：

1. 通过将“**启用安全性默认设置**”切换为“**否**”，禁用 [Azure 安全性默认设置](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)。

    a. 以安全管理员、条件访问管理员或全局管理员的身份登录到 Azure 门户。<BR/>
    b. 浏览到 Azure Active Directory >“ **属性**”。<BR/>
    c. 选择“**管理安全性默认设置**”。<BR/>
    d. 将“**启用安全性默认设置**”设置为“**否**”。<BR/>
    e. 选择“**保存**”。

2. 在许可邮箱上[启用客户端 SMTP 提交](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes)。

    a. 从 Microsoft 365 管理中心，转到“**活动用户**”并选择用户。<BR/>
    b. 转到“邮件”选项卡，然后在“**电子邮件应用**”下，选择“**管理电子邮件应用**”。<BR/>
    d. 确保已选中（已启用）“**已经过身份验证的 SMTP**”。<BR/>
    e. 选择“**保存更改**”。<BR/>

3. 在许可邮箱上 [禁用多重身份验证 (MFA)](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa)。

    a. 转到 Microsoft 365 管理中心，在左侧导航菜单窗格中选择“**用户**” > “**活动用户**”。<BR/>
    b. 选择“**多重身份验证**”。<BR/>
    c. 选择用户并禁用“**多重身份验证**”。<BR/>
