---
title: Outlook 桌面撤回或替换电子邮件
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687500"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>撤回或替换 Outlook 电子邮件

- 作为管理员，你可以**使用 PowerShell 代表用户撤回邮件**。 无法从管理中心撤回邮件。
- 您**只能撤回发送给组织中的人员的邮件**。 例如，如果邮件发送到 Gmail 地址，则无法撤回它。
- **只能撤回从电脑上的 Outlook 2016 发送的邮件**。 如果用户使用 Outlook for Mac 或 web 上的 Outlook 发送邮件，则无法撤回它。

若要撤回或替换电子邮件，请执行以下操作：

1. 在 Outlook 窗口左侧的文件夹窗格中，选择 "已发送邮件" 文件夹。
1. 双击要撤回的邮件以将其打开。
1. 选择 "**邮件**" 选项卡，然后选择 "**操作** > **撤回此邮件**"。
1. 选择 "**删除此邮件的未读副本**" 或 "**删除未读副本并将其替换为新邮件**"，然后选择 **"确定"**。
1. 如果要发送替换邮件，请撰写邮件，然后选择 "**发送**"。
1. 邮件撤回的成功或失败取决于收件人在 Outlook 中的设置。 有关检查召回的步骤，请参阅[本文](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)。

在组织中搜索和删除电子邮件

- 如果您不是全局管理员，则必须将您的帐户添加到电子数据展示管理器角色或合规性搜索管理角色中，才能搜索邮件。 若要删除邮件，您需要加入组织管理角色组或搜索和清除管理角色。 在[安全与合规中心](https://go.microsoft.com/fwlink/?linkid=2083731)中分配这些角色的权限。
- [创建内容搜索](https://docs.microsoft.com/office365/securitycompliance/content-search)以查找要删除的邮件。
- [连接到安全与合规中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)。

如果使用的是多重身份验证，请参阅[使用多重身份验证连接到 Microsoft 365 安全与合规中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)。