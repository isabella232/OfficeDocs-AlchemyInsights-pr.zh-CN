---
title: 反垃圾邮件 5.4.1 DBEB 捕获全部
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: 4f531a063d63aff239ef7dead869bb526e17fb35
ms.sourcegitcommit: 2591e1f56e8943bddb9d3b77ba5b494ac49d4f30
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/15/2019
ms.locfileid: "38672423"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>修复错误代码550的传递问题5.4.1 中继访问被拒绝

当您在进入 Office 365 网络时[检查电子邮件地址是否有效以防止 bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking)时，会出现此问题。 请尝试执行以下操作：

1. 确定问题是否特定于整个域或单个电子邮件地址：
    - 整个域：有时域需要同步;尝试[将域设置为 "内部"，然后再设置为 "权威"](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)。
    - 单个电子邮件地址：有时需要同步地址;更改 smtp 代理地址，然后将其更改为 "可帮助"。
2. 确定问题是否特定于组或公用文件夹。 对于某些对象类型，可能需要在 Azure Active Directory 中手动创建对象。

如果你需要其他帮助，请打开支持票证并指定问题的范围（includidng 要发送到的对象的类型），以便我们可以为你提供更好的帮助。