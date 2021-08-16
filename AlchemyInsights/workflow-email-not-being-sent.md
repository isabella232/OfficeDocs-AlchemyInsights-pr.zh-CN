---
title: 未发送工作流电子邮件
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 2caf8e0878da0049667d9a19f4488eaec4b9327fbf36be7d29dbf4b7a9c89158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072510"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>未针对列表或库SharePoint工作流电子邮件

1. 来自工作流的电子邮件不会发送给所有用户或仅发送给特定用户，或者您看到无法发送电子邮件的错误。请确保电子邮件具有 **有效的收件人**。

    检查该用户是否存在于该网站集的"所有 (权限") 列表中。  示例直接 URL：https:// <tenant> .sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx？MembershipGroupId=0

    - 如果用户不存在，请确保用户已登录到页面。 
    - 如果是外部用户，请确保已接受其邀请。
    - 如果用户存在于权限组中，请确保电子邮件地址正确。
    - 如果未在此处设置用户电子邮件地址，则为该用户创建示例警报，以强制将用户帐户从用户配置文件同步到SharePoint网站集。
 
2. 来自工作流的电子邮件将发送给网站集管理员，而不是发送给其他用户，并看到 HTTP 禁止 **<span>https</span>错误：//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**。
 

    请参阅[在向组发送电子邮件时拒绝SharePoint访问](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)。

    此外，验证 **"受限访问用户权限锁定模式** "网站集功能是否未处于活动状态。


## <a name="related-topics"></a>相关主题
想要尝试在 Microsoft Flow Online SharePoint？
- [创建Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 和 Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


