---
title: Outlook桌面重新调用或替换电子邮件
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 33fe7ebd53d7ff11dbab54ce589aaf58e68c633be4d83a3cdfb00edc7752430e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918385"
---
# <a name="recall-or-replace-an-outlook-email-message"></a>重新调用或Outlook电子邮件

- 作为管理员，可以使用 **PowerShell 代表用户撤回邮件**。 无法从管理中心撤回邮件。
- 只能 **撤回发送给组织成员的邮件**。 例如，如果邮件已发送到 Gmail 地址，则你无法撤回它。
- 你 **只能撤回从电脑上Outlook 2016发送的消息**。 如果用户使用 Outlook for Mac 或 Outlook 网页版 发送邮件，则不能撤回它。

重新调用或替换电子邮件：

1. 在"已发送邮件"窗口左侧Outlook，选择"已发送项目"文件夹。
1. 双击要撤回的邮件以打开它。
1. 选择"**邮件"** 选项卡，然后选择"**操作**  >  **""撤回此邮件"。**
1. 选择 **"删除此邮件的** 未读副本"或"删除 **未** 读副本并替换为新邮件"，然后选择"确定 **"。**
1. 如果要发送替换邮件，请撰写邮件，然后选择"发送 **"。**
1. 邮件撤回是成功还是失败取决于收件人在邮件Outlook。 有关检查撤回的步骤，请参阅 [本文](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)。

在组织中搜索并删除电子邮件

- 如果你不是全局管理员，则必须将你的帐户添加到电子数据展示管理员角色或合规性搜索管理角色中才能搜索邮件。 若要删除邮件，需要加入组织管理角色组或搜索和清除管理角色。 这些角色的权限在安全与合规 [中心内分配](https://go.microsoft.com/fwlink/?linkid=2083731)。
- [创建内容搜索](https://docs.microsoft.com/microsoft-365/compliance/content-search) 以查找要删除的邮件。
- [连接安全与合规中心 PowerShell。](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)

如果你使用的是多重身份验证，请参阅连接身份验证Microsoft 365安全与合规中心[PowerShell。](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)