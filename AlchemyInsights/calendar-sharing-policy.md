---
title: 618 日历共享策略
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091583"
---
# <a name="policy-error-when-sharing-a-calendar"></a>共享日历时出现策略错误

1. 根据你的情况执行下列操作之一：
    - 连接远程Exchange Online PowerShell 进行连接。 有关详细信息，请参阅[连接Exchange Online PowerShell 进行远程访问](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)。
    - 在本地服务器上，打开命令行管理Exchange命令行管理程序。
2. 确定分配给用户的共享策略。 为此，请运行以下命令并记下返回的策略：

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. 更新用户的共享策略。 为此，请按照下列步骤操作：
    - 打开“Exchange 管理中心”。
    - 单击 **"** 组织"，然后双击"单个共享"下分配给 **用户的策略**。 这是步骤 2 中返回的策略。
    - 在"共享规则"页上的"指定要共享的信息"下，选择要允许的 **日历共享级别**;单击"**保存"。**

有关详细信息，请参阅：当用户尝试共享日历时，"策略不允许向一个或多个收件人授予此级别的权限 [ () "错误](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)。
