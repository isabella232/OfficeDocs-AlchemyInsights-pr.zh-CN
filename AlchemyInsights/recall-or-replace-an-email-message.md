---
title: 重新调用或替换电子邮件
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024376"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>重新调用或替换电子邮件Microsoft 365

- 只能 **撤回发送给组织成员的邮件**。 例如，如果邮件发送到 Gmail 地址，则你无法撤回它。
- 你 **只能从电脑的 Outlook中撤回邮件**。 如果用户使用 Outlook for Mac 或 Outlook 网页版 发送邮件，则不能撤回它。
- 作为租户管理员，您可以使用 **PowerShell** (代表用户检索邮件。有关详细信息，请参阅：搜索并删除) 。 [](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)
- 无法从管理中心撤回邮件。 有关详细信息，请向下滚动到"搜索并删除您组织的电子邮件"。

**重新调用或替换你发送的电子邮件**

1. 在"已发送邮件"窗口左侧Outlook，选择"已发送项目"文件夹。
2. 打开要撤回的邮件。 必须双击以打开邮件。 选择邮件以便显示在阅读窗格中将不允许您撤回邮件。
3. 从"邮件"选项卡中，选择 **"操作**  >  **""撤回此邮件"。**
4. 选择 **"删除此邮件的未读** 副本"或"**删除未** 读副本并替换为新邮件"，然后选择"确定 **"。**
5. 如果要发送替换邮件，请撰写邮件，然后选择"发送 **"。**
6. 邮件撤回是成功还是失败取决于收件人在邮件Outlook。

有关详细信息，包括如何检查撤回，请参阅 [重新调用或替换你发送的电子邮件](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)。

***若要在组织中搜索和删除电子邮件***，如果你是全局管理员，则最为简单。如果你不是全局管理员，则必须将你的帐户添加到电子数据展示管理员角色组或合规性搜索管理角色。 若要删除邮件，需要加入组织管理角色组或搜索和清除管理角色。 这些角色的权限在安全与合规中心 [&分配](https://protection.office.com/)。

1. [创建内容搜索](https://docs.microsoft.com/microsoft-365/compliance/content-search) 以查找要删除的邮件。
2. [连接到安全与合规中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)。

如果你使用 MFA (多重身份验证) ，请参阅 连接 to Microsoft 365 Security [& Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)。
