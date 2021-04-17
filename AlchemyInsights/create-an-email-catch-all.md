---
title: 创建电子邮件捕获全部
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
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816190"
---
# <a name="create-an-email-catch-all"></a>创建电子邮件捕获全部

强烈建议不要使用 catch all。 最好向发件人提供退回邮件，让发件人知道他们的邮件无法以地址方式传递，以便可以采取措施。 您还可以将受监视的邮箱限制为仅捕获以前有效的电子邮件地址。 

任何捕获所有邮箱都将收到大量垃圾邮件，如果未受到密切监视，最终可能会填充这些垃圾邮件。  (有接收限制。)  

如果您决定继续，请按照以下步骤操作：

1. 创建包含"所有&"的动态通讯组。

2. 创建专用邮箱以捕获电子邮件，例如，catchall@domain.com。

3. 对于特定域，将 DomainType 设置为"InternalRelay"。 如果稍后删除 catch all，请确保将域设置回"权威"。

4. 创建邮件流传输规则，如下所示：

    - 如果发件人为"组织外部"
    - 将邮件重定向到 Catchall@domain.com
    - 除非收件人是通讯组的成员 allusers@domain.com (通讯组包含所有) 
    - 确保验证是否将新邮箱添加到动态通讯组
