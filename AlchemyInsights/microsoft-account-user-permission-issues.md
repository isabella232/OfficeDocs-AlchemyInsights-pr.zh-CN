---
title: 疑难解答 - 在目录中找不到用户
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098160"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>疑难解答 - 在目录中找不到用户

如果用户在目录中收到错误消息"找不到用户"，请重试，其中问题类型为"不在目录中的用户"。

可以完成以下步骤来解决问题。

- 确保接受电子邮件邀请的帐户与以后用于登录的帐户相同。 确保用户使用相同的帐户接受邀请并登录到网站。 

有关详细信息，请参阅[如何管理 Microsoft 帐户的别名以管理Microsoft 365 </a> 登录](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)。 

- 浏览到 () 收到错误的每个网站。 

将双引号 ("/_layouts/15/people.aspx/membershipgroupid=0") 添加到网站 URL 的末尾。 

示例：https：//<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0。

- 从列表中选择用户。

- 单击 **"从功能区删除** 用户权限"。 
-  添加回"用户"，再将邀请重新发送给用户。

