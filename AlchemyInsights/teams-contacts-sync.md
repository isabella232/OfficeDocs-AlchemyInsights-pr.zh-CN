---
title: Teams 联系人同步
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
- "9004610"
- "11540"
ms.openlocfilehash: efc1f29c6e2f76d763f2f8102db7e9f6afb1f1be
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327323"
---
# <a name="teams-contacts-sync"></a>Teams 联系人同步

Teams 使用组织 Active Directory 中的联系人和添加到用户的 Outlook 默认文件夹的联系人。 如果联系人未显示在 Microsoft Teams 中，请尝试以下操作：

**注意：** 如果最近更新了一个或多个联系人的信息，则联系人可能需要 48 小时才能同步。

1. 退出 Teams 并重启。 检查联系人是否显示。
1. 清除 Teams 缓存：
    1. 浏览到 **%appdata%\Microsoft\Teams**。
    1. 删除文件夹的内容。
    1. 重启计算机，然后启动 Teams。
1. 如果联系人位于 Outlook 中，请确保将其添加到联系人列表。 在 Outlook 的地址栏中，选择“**文件**”，然后选择“**添加到联系人**”。
1. 确保用户的 Exchange 邮箱在线托管（而不是本地）。 有关详细信息，请参阅 [Exchange 与 Microsoft Teams 如何交互](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)。
1. 确保将联系人的电话号码添加到联系人信息中。
1. 在搜索栏中搜索联系人的电子邮件。 将可以检索到的联系同步到联系人列表。
