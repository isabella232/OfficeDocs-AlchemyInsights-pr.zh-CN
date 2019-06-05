---
title: 创建和使用共享邮箱
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 1825cfd0a78a29734d0a5128e19acbfba9115d32
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2019
ms.locfileid: "34717337"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>问题疑难解答-在目录中找不到用户

<p>如果用户收到错误消息<strong> &ldquo; &hellip;, 则无法&rsquo;在目录中找到用户。请稍后重&hellip;试</strong>问题类型为<strong> &ldquo;"用户不在目录中&rdquo;</strong>" 的。, 可以完成以下步骤以解决问题。</p> <ol> <li>确保接受电子邮件邀请的帐户是以后用于登录的帐户。 请确保用户使用相同的帐户接受邀请并登录网站。 <br /><br />有关详细信息, 请参阅<a href="https://support.microsoft.com/en-us/help/12407/microsoft-account-how-to-manage-aliases">如何管理你的 Microsoft 帐户的别名</a>以管理 Office 365 登录名。 <br /><br /></li> <li>浏览到用户收到错误的每个站点。 <br /><br />a. 将<strong> &ldquo;/_layouts/15/people.aspx/membershipgroupid = 0&rdquo; </strong> (在双引号内) 添加到网站 URL 的末尾。 <br /><br />示例: https://&lt;contoso&gt;. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0 <br /><br />b. 从列表中选择用户。 <br /><br />c. 单击<strong>功能区中的 "删除用户权限"</strong>。 <br /><br />d. 重新添加用户并将邀请重新发送给用户。</li> </ol>

