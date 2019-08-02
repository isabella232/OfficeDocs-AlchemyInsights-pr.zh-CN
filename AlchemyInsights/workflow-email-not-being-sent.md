---
title: 未发送工作流电子邮件
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059594"
---
# <a name="workflow-email-is-not-being-sent"></a>未发送工作流电子邮件

1. 来自工作流的电子邮件不会发送给所有用户或仅发送给特定用户, 也不会看到错误**电子邮件无法发送。请确保电子邮件具有有效的收件人**。

检查用户是否存在于该网站集的 "**所有人员**权限" 组 ("用户信息" 列表中)。  示例直接 URL: https://<tenant>sharepoint.com/sites/<sitename>/_layouts/15/people.aspx？MembershipGroupId = 0

- 如果用户不存在, 请确保用户已登录到页面。 
- 如果是外部用户, 请确保已接受其邀请。
- 如果用户在权限组中确实存在, 请确保电子邮件地址正确无误。
- 如果未在此处设置用户电子邮件地址, 则为该用户创建一个示例通知, 以强制将该用户帐户从 SharePoint 的用户配置文件同步到此网站集。
 
2. 来自工作流的电子邮件将发送给网站集管理员, 而不是发送给其他用户, 并查看错误**HTTP 禁止访问<spam> <spam>。 ** <spam> <spam>
 

请参阅向[组发送电子邮件时访问被拒绝](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups)。

此外, 确认 "**受限访问用户权限锁定模式**" 网站集功能未处于活动状态。

## <a name="related-topics"></a>相关主题
- [创建流](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 和流](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


