---
title: 618日历共享策略
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
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684220"
---
# <a name="policy-error-when-sharing-a-calendar"></a>共享日历时出现策略错误

1. 根据您的具体情况执行下列操作之一：
    - 使用远程 PowerShell 连接到 Exchange Online。 有关详细信息，请参阅 [使用远程 PowerShell 连接到 Exchange Online](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)。
    - 在本地服务器上，打开 Exchange 命令行管理程序。
2. 确定分配给用户的共享策略。 为此，请运行以下命令并记下返回的策略：

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. 为用户更新共享策略。 为此，请按照下列步骤操作：
    - 打开“Exchange 管理中心”。
    - 单击 " **组织**"，然后双击在 **单独共享**中分配给用户的策略。 这是在步骤2中返回的策略。
    - 在 "共享规则" 页上的 " **指定要共享的信息**" 下，选择要允许的日历共享级别;单击 " **保存**"。

有关详细信息，请参阅： ["策略不允许在此级别将权限授予一个或多个收件人 (s) " 在用户尝试共享日历时出错](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)。
