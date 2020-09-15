---
title: 创建电子邮件全部捕获
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
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712976"
---
# <a name="create-an-email-catch-all"></a>创建电子邮件全部捕获

强烈建议不要使用全部捕获。 更好的方法是，让发件人向发件人告知其邮件无法按寻址方式传递，这样他们就可以采取措施。 您还可以将受监视的邮箱限制为仅捕获以前有效的电子邮件地址。 

任何捕获所有邮箱都将收到大量垃圾邮件，并且最终可能会填写（如果未受到严密监控）。  (有接收限制。 )  

如果你决定继续，请按照以下步骤操作：

1. 创建动态通讯组，& 包括 "所有收件人类型"。

2. 创建专用邮箱来捕获电子邮件，例如，catchall@domain.com。

3. 对于特定域，将 DomainType 设置为 "InternalRelay"。 如果稍后删除 "全部捕获"，请务必将域重新设置为权威。

4. 创建邮件流传输规则，如下所示：

    - 如果发件人是 "组织外部"
    - 将邮件重定向到 Catchall@domain.com
    - 除非收件人是 allusers@domain.com 的成员 (通讯组包含所有成员) 
    - 确保新邮箱已添加到动态通讯组中
