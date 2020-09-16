---
title: 问题疑难解答-在目录中找不到用户
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725397"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>问题疑难解答-在目录中找不到用户

如果用户在目录中收到错误消息 "找不到用户"，请重试问题类型为 "用户不在目录中的用户"。

若要解决问题，可以完成以下步骤。

- 确保接受电子邮件邀请的帐户是以后用于登录的帐户。 请确保用户使用相同的帐户接受邀请并登录网站。 

有关详细信息，请参阅 [如何管理你的 microsoft 帐户的别名 </a> 以管理 microsoft 365 登录名](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)。 

- 浏览到用户收到错误的每个站点 (s) 。 

将 "/_layouts/15/people.aspx/membershipgroupid = 0" (在双引号内添加到网站 URL 的末尾) 。 

示例： https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0。

- 从列表中选择用户。

- 单击功能区中的 " **删除用户权限** "。 
-  重新添加用户并将邀请重新发送给用户。

