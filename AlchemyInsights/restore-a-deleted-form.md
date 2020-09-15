---
title: 还原已删除的窗体
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2547"
- "9000672"
ms.openlocfilehash: 6923c15c3cce90c98ae79181e978fba273ab6059
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662414"
---
# <a name="restore-a-deleted-form"></a>还原已删除的窗体

如果您意外删除了 Microsoft Forms 中的表单，可以对其进行恢复。 以已删除表单的所有者的形式登录 Microsoft 表单。 选择 " **回收站**"，然后选择要恢复的表单并选择 " **还原**"。 还原后，选择 " **返回我的窗体" 页面** 箭头。

只有表单的所有者可以将其恢复。 如果表单所有者的帐户已被禁用或从租户中删除，则只有全局管理员可以恢复该表单。 全局管理员必须具有表单许可证才能执行还原。 只有在30天内被禁用或从租户中删除的用户帐户中创建的表单可以还原。

如果您是租户的全局管理员，并且想要从已删除或已禁用的帐户中恢复表单，请将 [电子邮件地址] 替换为以下 URL 中已删除或已禁用用户的电子邮件地址： ** https://forms.office.com/Pages/delegatepage.aspx?originalowner= [电子邮件地址]** 例如，如果您的电子邮件地址是 JOHNDOE@CONTOSO.COM，则 URL 将为： **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com** 。 

一旦您有权访问用户的已删除窗体，请选择要移动的窗体，然后选择 "**更多表单操作**  >  **移动**"。

如果要恢复已删除且已从组织中删除用户的表单，全局管理员可以选择恢复用户、重置该用户的密码，然后以该用户身份登录，然后访问该表单以将其移动到其他活动用户。 