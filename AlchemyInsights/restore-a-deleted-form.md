---
title: 还原已删除的表单
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2547"
- "9000672"
ms.openlocfilehash: 48018accc23a504c34b5469c198d6f29929d25c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809465"
---
# <a name="restore-a-deleted-form"></a>还原已删除的表单

如果意外删除了 Microsoft Forms 中的窗体，可以恢复它。 以已删除表单的所有者的形式登录 Microsoft Forms。 选择 **回收站**，然后选择要恢复的表单，然后选择"还原 **"。** 还原后，选择" **返回我的窗体"页** 箭头。

只有表单的所有者才能恢复它。 如果表单所有者的帐户被禁用，或者已从租户中删除，则只有全局管理员才能恢复表单。 全局管理员必须具有表单许可证才能执行还原。 只能还原在用户帐户被禁用或删除后 30 天内创建的表单。

如果您是租户的全局管理员，并且希望从已删除或禁用的帐户恢复表单，请将 [电子邮件地址] 替换为以下 URL 中已删除或已禁用用户的电子邮件地址：[**https://forms.office.com/Pages/delegatepage.aspx?originalowner= 电子邮件地址]** 例如，如果您的电子邮件地址为 johndoe@contoso.com，则 URL 为： **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com** 。 

有权访问用户的已删除窗体后，选择要移动的窗体，然后选择"移动 **更多窗体操作**  >  **"。**

如果要恢复已删除表单且用户已从组织中删除的表单，全局管理员可以选择恢复用户，重置该用户的密码，然后在以该用户身份登录时，访问表单以将其移动到另一个活动用户。 