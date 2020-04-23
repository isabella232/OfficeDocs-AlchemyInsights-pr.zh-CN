---
title: 撤回或替换电子邮件
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: e541620a499b02a7206579ffcc505ceb4e632a4c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742745"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>在 Microsoft 365 中撤回或替换电子邮件

- 您**只能撤回发送给组织中的人员的邮件**。 例如，如果邮件发送到 Gmail 地址，则无法撤回它。
- 您**只能撤回从 Outlook 2016 为电脑发送的邮件**。 如果用户使用 Outlook for Mac 或 web 上的 Outlook 发送邮件，则无法撤回它。
- 如果您是管理员，则可以**使用 PowerShell 代表用户撤回邮件**。 无法从管理中心撤回邮件。 向下滚动到 "搜索组织中的电子邮件并删除电子邮件"，了解详细信息。

**撤回或替换您发送的电子邮件**

1. 在 Outlook 窗口左侧的文件夹窗格中，选择 "已发送邮件" 文件夹。
2. 打开要撤回的邮件。 您必须双击才能打开邮件。 如果选择邮件使其显示在阅读窗格中，则不会允许您撤回邮件。
3. 从 "邮件" 选项卡中，选择 "**操作** > **撤回此邮件**"。
4. 选择 "**删除此邮件的未读副本**" 或 "**删除未读副本并将其替换为新邮件**"，然后选择 **"确定"**。
5. 如果要发送替换邮件，请撰写邮件，然后选择 "**发送**"。
6. 邮件撤回的成功或失败取决于收件人在 Outlook 中的设置。

有关详细信息，包括如何检查撤回，请参阅[撤回或 replace 您发送的电子](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)邮件。

***在组织中搜索和删除电子邮件***若要在组织中搜索和删除电子邮件，您是全局管理员的最简单方法。如果您不是全局管理员，则必须将您的帐户添加到电子数据展示管理器角色组或合规性搜索管理角色。 若要删除邮件，您需要加入组织管理角色组或搜索和清除管理角色。 对这些角色的权限是在[安全 & 合规中心](https://protection.office.com/)中分配的。

1. [创建内容搜索](https://docs.microsoft.com/office365/securitycompliance/content-search)以查找要删除的邮件。
2. [连接到安全与合规中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)。 

如果使用的是 MFA，请参阅[使用多重身份验证连接到 Microsoft 365 security & 合规性中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)。 
