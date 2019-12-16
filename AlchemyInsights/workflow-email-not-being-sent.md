---
title: 未发送工作流电子邮件
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049363"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>未向 SharePoint 列表或库发送工作流电子邮件

1. 来自工作流的电子邮件不会发送给所有用户或仅发送给特定用户，也不会看到错误**电子邮件无法发送。请确保电子邮件具有有效的收件人**。

    检查用户是否存在于该网站集的 "**所有人员**权限" 组（"用户信息" 列表中）。  示例直接 URL： https://<tenant><sitename>/_layouts/15/people.aspx？MembershipGroupId = 0

    - 如果用户不存在，请确保用户已登录到页面。 
    - 如果是外部用户，请确保已接受其邀请。
    - 如果用户在权限组中确实存在，请确保电子邮件地址正确无误。
    - 如果未在此处设置用户电子邮件地址，则为该用户创建一个示例通知，以强制将该用户帐户从 SharePoint 的用户配置文件同步到此网站集。
 
2. 来自工作流的电子邮件将发送给网站集管理员，而不是发送给其他用户，并查看错误**HTTP 禁止访问<span>https：</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.sendemail**。
 

    在向[SharePoint 组发送电子邮件时，请参阅访问被拒绝](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)。

    此外，确认 "**受限访问用户权限锁定模式**" 网站集功能未处于活动状态。


## <a name="related-topics"></a>相关主题
想要在 SharePoint Online 中试用 Microsoft 流吗？
- [创建流](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 和流](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


