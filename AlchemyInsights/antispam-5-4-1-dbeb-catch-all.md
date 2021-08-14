---
title: AntiSpam 5.4.1 DBEB catch-all
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
- "9001209"
- "3167"
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932267"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>修复错误代码为 550 5.4.1 中继访问被拒绝的传递问题

在 [检查电子邮件地址是否](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) 有效以防止在进入 Microsoft 网络时发生回弹时，会出现此问题。 请尝试执行以下操作：

1. 确定问题是特定于整个域还是单个电子邮件地址：
    - 整个域：有时需要同步域;尝试[将域设置为"内部"，然后返回到"权威"。](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains)
    - 单个电子邮件地址：有时需要同步地址;更改 smtp 代理地址，然后再更改回地址可能会有所帮助。
2. 确定问题是特定于组还是公用文件夹。 对于一些对象类型，可能需要手动在 Azure Active Directory。

如果需要其他帮助，请打开支持票证并指定问题范围 (包括你发送到项目的对象类型) 以便我们可以更好地协助你。