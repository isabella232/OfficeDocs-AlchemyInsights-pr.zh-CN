---
title: 意外的多重身份验证
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: 8a912b32dee23e8c6eae0ad7bc72228d49ceeb92
ms.sourcegitcommit: 4f7ff981bbb3a98663cd164d0a10bb082cdf7ec9
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2020
ms.locfileid: "42946611"
---
# <a name="unexpected-multi-factor-authentication"></a>意外的多重身份验证

如果你的租户在 2019 年 10 月 21 日后创建，并且意外收到了有关 MFA 的提示，则你的租户中可能启用了[安全性默认值](http://aka.ms/securitydefaults)。 

要管理安全性默认值：

1. 使用全局管理员凭据登录[管理中心](https://go.microsoft.com/fwlink/p/?linkid=834822)。

2. 转到 [Azure Active Directory 属性](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)。

3. 在页面底部，单击“**管理安全性默认值**”。

4. 单击“**是**”启用安全性默认值，或单击“**否**”禁用安全性默认值。
